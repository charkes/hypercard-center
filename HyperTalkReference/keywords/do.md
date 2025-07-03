---
title: do
card_id: 25485
modified: yes
---

# do

`do [ph:expression] [as [ph:scriptLanguage]]`

The `do` keyword forces HyperCard to evaluate `[ph:expression]` and to send the result as a message to the current card.

The value of `[ph:expression]` can contain more than one line. For example, if you have a series of statements in a card field called Example, HyperCard will apply `do` to each line:

`do card field "Example"`

When you use the `as [ph:scriptLanguage]` form, HyperCard executes the script in `[ph:expression]` using the OSA-compliant scripting component named in `[ph:scriptLanguage]`:

```
do field 1 as AppleScript
do theScript as UserTalk
```

You can also send `do` from the Message box.

## Demo Script

```
on doLast3Lines
  put the number of lines of bkgnd field "Demo Script" into N
  do line (N - 2) to N of bkgnd field "Demo Script"
end doLast3Lines

put sqrt(2)
beep
flash
```

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

## Related Topics

* [value](/HyperTalkReference/functions/value)
