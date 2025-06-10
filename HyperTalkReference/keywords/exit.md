---
title: exit
card_id: 25835
modified: yes
---

# exit

<code><pre>
exit repeat
exit <i>functionName</i>
exit <i>messageName</i>
exit to HyperCard
</pre></code>

<br>
The<code> exit </code>keyword interrupts the current flow of control.<br>
<br>
<code>Exit repeat </code>sends control to the end of a<code> repeat </code>structure, ending execution of the loop regardless of the state of the controlling conditions.<br>
<br>
The<code> exit <i>functionName</i> </code>and<code> exit <i>messageName</i> </code>forms stop the current message or function handler. Control  returns to any pending statements from another handler, if any.<br>
<br>
<code>Exit to HyperCard </code>terminates all running or pending handlers and cancels all pending messages.<br>
<br>
Using<code> exit </code>to leave a function handler sets the value of the function to empty.<br>

## Examples

```
if N = 0 then exit repeat

if it is empty then exit mySave

if there is no card field "Index" then exit indexFunction

-- In the following example, the openCard message will not occur as the 
-- user goes from card to card:

on closeCard
  flash
  exit to HyperCard
end closeCard

on openCard
  beep
end openCard

-- The newButton message will occur because HyperCard sends it before
-- the exit to HyperCard:

on anExample
  doMenu "New Button" -- creates a new button, sends newButton message
  exit to HyperCard
end anExample

on newButton
  beep
end newButton
```

## Demo Script

<code><pre>
on exitDemo
  answer "Would you like to see a demo?" with "No" or "Yes"
  if it is "No" then exit exitDemo
  put "Click the mouse to exit this handler…"
  put 1 into lineNum
  put the number of lines in me into totalLines
  set the autoSelect of me to true -- to get a nice solid hilite
  repeat
    if lineNum > totalLines then put 1 into lineNum
    select line lineNum of me
    if the mouseClick then <b>exit</b> <b>repeat</b>
    add 1 to lineNum
  end repeat
  wait 20
  select line 0 of me
  set the autoSelect of me to false
end exitDemo
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/functionName.md]

[embed:HelpExtras/Placeholders/messageName.md]

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
