---
title: answer
card_id: 30026
modified: yes
---

# answer

<code><pre>
answer <i>text</i>

answer <i>text</i> with <i>reply1</i>
answer <i>text</i> with <i>reply1</i> or <i>reply2</i>
answer <i>text</i> with <i>reply1</i> or <i>reply2</i> ¬
   or <i>reply3</i>

answer file <i>text</i> [of type <i>fileType</i>]

answer program <i>text</i> [of type ¬
 <i>processType</i>]
</pre></code>


The form<code> answer <i>text</i> </code> displays a <b>question</b> (<i><code>text</i></code> ) in a dialog box. The dialog box contains from one to three buttons, each representing a different  reply the user can select.

If you use<code> answer </code>without specifying any replies, HyperTalk displays an OK button as the default. Otherwise, the last reply you specify becomes the default button. (Pressing Enter or Return chooses the default button.)<code> Answer </code>returns the name of the button clicked by the user in the local variable<code> it</code>.

<code>Answer </code>automatically sizes the dialog box to fit the size of the text (up to 13 lines). The total length of the text cannot exceed 254 characters.

The form `Answer file <i>text</i>` displays a directory dialog box that you use to select a file.

`answer file <i>text</i> of type <i>fileType</i>`  displays only files of a specified type: `application`, `picture`, `painting` or `paint`, `stack`, or `text`. (Click the <i>fileType</i> placeholder for more information about file types.)

`Answer file` returns the full pathname of the selected file in the local variable `it`. It returns empty if the user clicks Cancel.

`Answer file` also sets the `result` to `Cancel` if the user clicks Cancel. Check the value of `the result` in the statement immediately following `answer file`.

The form `Answer program <i>text</i>` produces a dialog box of all System 7-friendly processes currently running on the local machine and on any networked computers to which the local machine has access.

A System 7-friendly process is a program or entity that’s capable of exchanging information with another process. The name of the selected program is placed in the container `it`.

`<i>text</i>` is a quoted prompting string that appears at the top of the dialog box. If you provide the null string for `<i>text</i>`  (that is, `""`), the system puts `Choose a program to link to:` at the top of the dialog box.

Use the form `answer program <i>text</i> of type <i>processType</i>`  to see only certain types of processes (spell checkers, word processors, spreadsheets, and so on).

An application's default process type is its creator. So to see only copies of HyperCard, you’d use WILD.

For more details, see "PPC Toolbox" in Inside <i>Macintosh V.6</i> or <i>Inside Macintosh: Interapplication Communications</i>.

## Examples

```
answer "The file has been saved."
answer "Really delete this file?" with "Yes" or "No"
answer "Sort by:" with "Cancel" or "Number" or "Name"

answer file "Choose a file to load:"
answer file "Where is the stack you want?" of type stack

answer file "Where is the program you want to open?" of type application
if the result is "Cancel" then ...

answer program "What program do you want to switch to?"
answer program "" -- prompts with "Choose a program to link to:"
```

## Demo Script

<code><pre>
on mouseUp
  <b>answer</b> file "Please select a file:" of type stack OR text
  if it is not empty then
    put it into fullPathName
    put fullPathToFileName(fullPathName) into fileName -- see below
    <b>answer</b> "You selected file: “" & fileName & "”" & return & return &¬
    "The full path for the file is:" & return & "“" & fullPathName & "”"
  end if
end mouseUp

function fullPathToFileName fullPathName
  put the itemDelimiter into savedDelimiter
  set itemDelimiter to ":"
  put last item of fullPathName into fileName
  set itemDelimiter to savedDelimiter
  return fileName
end fullPathToFileName
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/text.md]

[embed:HelpExtras/Placeholders/fileType.md]

## Related Topics

* [ask](/HyperTalkReference/commands/ask)
* [programs](/HyperTalkReference/functions/programs)
