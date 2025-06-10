---
title: subtract
card_id: 49191
---

# subtract

<code><pre>
subtract [ph:number] from [[ph:chunk] of] ¬
          [ph:container]
</pre></code>

where <code>[ph:container]</code> or <code>[ph:chunk]</code> must contain a number.

The <code>subtract</code> command subtracts <code>[ph:number]</code> from the specified container (or chunk) and puts the result into the container (or chunk), replacing what was there.

(You can use the <code>is a</code> operator to see if the container is a number.)

For example, if you say

<code><pre>
subtract 3 from theTotal
</pre></code>

and <code>theTotal</code> previously held 7, it will now hold 4.

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
