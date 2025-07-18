---
title: divide
card_id: 35162
---

# divide

```
divide [[ph:chunk] of] [ph:container] by [ph:number]
```

The `divide` command divides the number in the container or chunk by `[ph:number]` and puts the result into the container.

Dividing by 0 places `INF` (for infinity) into the chunk or container. Division is carried out to a precision of up to 19 decimal places.

Note: The container or chunk referred to must contain a number.

If the result is put into a field or the Message box, it is displayed according to the global property `numberFormat`.

(You can use the `is a` operator to see if the container is a number.)

## Examples

```
divide field "Total" by 100

divide line 10 of theTotal by (the number of lines of theTotal)

if theTotal is a number then divide theTotal by theNumberOfEntries
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [multiply](/HyperTalkReference/commands/multiply)
* [numberFormat](/HyperTalkReference/properties/numberFormat)
* [sqrt](/HyperTalkReference/functions/sqrt)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
