---
title: ask
card_id: 31208
modified: yes
---

# ask

<code><pre>
ask [ph:text1] [with [ph:text2]]

ask password [clear] [ph:text1] [with [ph:text2]]
ask file [ph:text1] [with [ph:fileName]]
</pre></code>


The <code>ask</code> command displays a <b>question</b> (<code>[ph:text1]</code>) in a dialog box along with a text box where the user can type a reply. The <code>ask</code> dialog automatically provides the OK and Cancel buttons.

You can supply a <b>default reply</b> using the <code>with [ph:text2]</code> option. The default text appears highlighted in the text box.

<code>Ask</code> returns the text entered by the user, if any, in the local variable <code>it</code>. If the user clicks Cancel, <code>ask</code> places <code>empty</code> in <code>it</code>.

<code>Ask </code>also sets the HyperTalk function <code>the result</code> to <code>empty</code> if the user clicks OK or to <code>Cancel</code>if the user clicks Cancel.  (So you can use the value of <code>the result</code> to determine whether the user provides an empty string or clicks Cancel.)  You must check <code>the result</code> in the statement immediately after the <code>ask</code> command.

Note: `ask` automatically sizes the dialog box to fit the size of the text (up to thirteen lines). The total length of the text cannot exceed 254 characters for both the prompt and the default reply.

`Ask password` displays a bullet (&bull;) for each character the user types and encrypts the reply as a number. You can save this number in a field to compare with future passwords. (The `ask password clear` form does [ph:not] encrypt the reply, but it [ph:does]  display a bullet for each typed character.)

Note: `ask password` is different from setting the password of the stack with the Protect Stack dialog. With `ask password`, your handler must set and check any passwords.

`Ask file` displays a directory dialog box in which you type the name of a file. The `with [ph:filename]` option provides a default name that appears in the text box.

## Examples

```
-- userName is a global variable set up by the Home stack:
ask "Enter your name:" with userName

ask "What time of day?" with "Noon"
if the result is "Cancel" then
   -- the user clicked the Cancel button
else if it is empty then
   -- the user clicked OK with no answer
else
   -- the user clicked OK and provided an answer
end if

ask password "Enter your password:"
if it is in card field "passwords" then allowAccess
else go Home

ask file "Save the file as:" with "Untitled"
```

## Demo Script

<code><pre>
on mouseUp
  -- convert some arbitrary seconds to the date
  -- to get the date format as set for the system.
  put "1838246400" into someSeconds
  convert someSeconds to short date


  <b>ask</b> "Enter your birthday:" with someSeconds
  if the result is "Cancel" then answer "You clicked Cancel."
  else
    put convertBirthDayToDays(it) into numberOfDays
    if numberOfDays is not empty
    then answer "You are" && numberOfDays && "days old."
  end if
end mouseUp

function convertBirthDayToDays birthDay
  convert birthDay to seconds
  if the result is "invalid date" then beep
  else
    convert the date to seconds
    put it - birthDay into secondsOld
    return secondsOld / 86400 -- 86400 is the number of seconds in a day
  end if
end convertBirthDayToDays
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/fileName.md]

[embed:HelpExtras/Placeholders/filename.md]

## Related Topics

* [answer](/HyperTalkReference/commands/answer)
