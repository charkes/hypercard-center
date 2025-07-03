---
title: if (single-statement)
card_id: 26805
modified: yes
---

# if (single-statement)

```
if [ph:trueOrFalse] then [ph:statements] ¬
   [else [ph:statements]]

if [ph:trueOrFalse]
then [ph:statements]
[else if [ph:trueOrFalse]
then [ph:statements]]
[else [ph:statements]]
```

The single-statement `if` structure tests for a condition and executes <b>one</b> statement if the condition is true. You use the optional `else if` or `else` form to run other  blocks of code in case the  condition following `if` is false.

Because each part of a simple `if` structure is limited to one statement, you don't need an `end if` statement.

You can send a one-line `if` structure from the Message box.

## Examples

```
if it is empty then exit myHandler

ask file "Save information to file:"
if it is empty then exit myHandler
else saveFile it

ask file "Save information to file:"
if it is empty
then exit myHandler
else saveFile it
```

## Placeholders

[embed:HelpExtras/Placeholders/trueOrFalse.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
