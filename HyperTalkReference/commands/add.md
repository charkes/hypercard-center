---
title: add
card_id: 29791
---

# add

`add [ph:number] to [[ph:chunk] of] [ph:container]`

Note: The container or chunk referred to must contain a number.

The `add` command adds the value of `[ph:number]` to the number in a container or chunk and replaces the contents of the container or chunk with the result.

(You can use the `is a` operator to see if the container is a number.)

## Examples

```
add 3 to It  

add field "Amount" to field "Total"

get last line of card field "credits"
if it is a number then add it to item 1 of theTotal

if the Message box is a number then add 15 to Message box
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [subtract](/HyperTalkReference/commands/subtract)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
