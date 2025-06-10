---
title: global
card_id: 26361
modified: yes
---

# global

<code>global <i>variableList</i></code><br>
<br>
The<code> global </code>keyword makes a variable and its contents available to any handler in HyperCard. Changing the value of a global variable in any handler changes its value everywhere.<br>
<br>
Note: You must use the <code>global</code> keyword in <b>each handler</b> to declare the global variables you want to use.<br>
<br>
Global variables are not saved between sessions of HyperCard. Global variables are also lost under System 6's single Finder when a user (or handler) suspends HyperCard by launching another application with the<code> open </code>command.<br>

## Examples

```
global myVar

global pages,sections,chapters
```

## Demo Script

<code><pre>
on mouseUp
  <b>global</b> theName
  ask "What is your name?"
  if it is empty then exit mouseUp
  put it into theName
  answerReverseName
end mouseUp

on answerReverseName
  <b>global</b> theName
  repeat with i = the number of chars in theName down to 1
    put char i of theName after reverseName
  end repeat
  answer "Your name spelled backwards is" && reverseName & "."
  -- put empty into the global when you are done with it:
  put empty into theName
end answerReverseName
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/variableList.md]

## Related Topics

* [The building blocks](/HyperTalkReference/hypertalkbasics/The-building-blocks)
