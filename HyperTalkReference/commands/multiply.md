---
title: multiply
card_id: 41612
---

# multiply

<code><pre>
multiply [[ph:chunk] of] [ph:container] ¬
     by [ph:number]
</pre></code>

where [ph:container] or [ph:chunk] must contain a number. (You can use the <code>is a</code> operator to see if the container is a number.)

The <code>multiply</code> command multiplies the number in the container or chunk by <code>[ph:number]</code> and puts the result into the container or chunk. The result is calculated to a precision of up to 19 decimal places.

The result is displayed in a field or the Message box according to the global property <code>numberFormat</code>.

## Examples

```
multiply field "Total" by 100
multiply line 10 of theTotal by (the number of lines of theTotal)

if theTotal is a number then multiply theTotal by theNumberOfEntries
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [divide](/HyperTalkReference/commands/divide)
* [numberFormat](/HyperTalkReference/properties/numberFormat)
* [sqrt](/HyperTalkReference/functions/sqrt)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
