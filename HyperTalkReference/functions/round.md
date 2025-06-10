---
title: round
card_id: 62709
---

# round

<code><pre>
the round of [ph:number]
</pre></code>

Value returned: the integer nearest to<code> [ph:number</code>]

Odd integers plus exactly 0.5 round up; even integers (or 0) plus exactly 0.5 round down. 

If <code>[ph:number]</code> is negative, HyperCard internally removes the negative sign, rounds its absolute value, then puts the negative sign back on. 


## Examples

```
the round of 5.5

the round of 5.5 + 3 -- returns 9
the round of (5.5 + 3) -- returns 8

get round(the top of card window / 2)
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [trunc](/HyperTalkReference/functions/trunc)
