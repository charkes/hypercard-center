---
title: global
card_id: 26361
modified: yes
---

# global

`global [ph:variableList]`

The `global` keyword makes a variable and its contents available to any handler in HyperCard. Changing the value of a global variable in any handler changes its value everywhere.

Note: You must use the `global` keyword in <b>each handler</b> to declare the global variables you want to use.

Global variables are not saved between sessions of HyperCard. Global variables are also lost under System 6's single Finder when a user (or handler) suspends HyperCard by launching another application with the `open` command.

## Examples

```
global myVar

global pages,sections,chapters
```

## Demo Script

```
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
```

## Placeholders

[embed:HelpExtras/Placeholders/variableList.md]

## Related Topics

* [The building blocks](/HyperTalkReference/hypertalkbasics/The-building-blocks)
