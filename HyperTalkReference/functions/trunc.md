---
title: trunc
card_id: 66892
---

# trunc

<code><pre>
the trunc of [ph:number]
</pre></code>

Value returned: an integer equal to the integer part of<code> [ph:number</code>]. Any fractional part is disregarded, regardless of the number’s sign.  

Note: <code>trunc</code> returns correct values only for real numbers in the range -2,147,483,648 through 2,147,483,647 (the maximum long integer value). 


## Examples

```
the trunc of 5.9
the trunc of 5.9 + 3.1 -- returns 8.1
the trunc of (5.9 + 3.1) -- returns 9
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [round](/HyperTalkReference/functions/round)
