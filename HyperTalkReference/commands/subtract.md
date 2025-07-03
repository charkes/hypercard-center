---
title: subtract
card_id: 49191
---

# subtract

```
subtract [ph:number] from [[ph:chunk] of] ¬
          [ph:container]
```

where `[ph:container]` or `[ph:chunk]` must contain a number.

The `subtract` command subtracts `[ph:number]` from the specified container (or chunk) and puts the result into the container (or chunk), replacing what was there.

(You can use the `is a` operator to see if the container is a number.)

For example, if you say

```
subtract 3 from theTotal
```

and `theTotal` previously held 7, it will now hold 4.

## Examples

```
subtract 4 from bkgnd field "total"

subtract last line of card field "debits" from item 1 of theTotal

if the Message box is a number then subtract 15 from Message box
```

## Related Topics

* [add](/HyperTalkReference/commands/add)
* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
