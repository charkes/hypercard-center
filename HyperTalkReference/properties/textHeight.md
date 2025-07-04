---
title: textHeight
card_id: 85522
---

# textHeight

` set `[`the`]` textHeight to [ph:posInteger] set `[`the`]<code> textHeight of [ph:field] ¬     to [ph:posInteger]

</code>The `textHeight` property returns or sets the space, in pixels, between the baselines of Paint text or text in fields. (`TextHeight `doesn't apply to buttons because buttons can display only one line of text.)

The default value is the value of the `textSize` property plus one-third of that value. 

 You can’t set the `the textHeight` to a value less than the` textSize`.

The `textHeight` property affects a field only when the field’s `fixedLineHeight` property is true. 


## Examples

```
the textHeight of field 1

set the textHeight to 15 -- for the text tool
set the textHeight of field 1 to 12
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
* [textAlign](/HyperTalkReference/properties/textAlign)
* [textFont](/HyperTalkReference/properties/textFont)
* [textSize](/HyperTalkReference/properties/textSize)
* [textStyle](/HyperTalkReference/properties/textStyle)
