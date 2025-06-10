---
title: textHeight
card_id: 85522
---

# textHeight

<code> set </code>[<code>the</code>]<code> textHeight to [ph:posInteger] set </code>[<code>the</code>]<code> textHeight of [ph:field] ¬     to [ph:posInteger]

</code>The <code>textHeight</code> property returns or sets the space, in pixels, between the baselines of Paint text or text in fields. (<code>TextHeight </code>doesn't apply to buttons because buttons can display only one line of text.)

The default value is the value of the <code>textSize</code> property plus one-third of that value. 

 You can’t set the <code>the textHeight</code> to a value less than the<code> textSize</code>.

The <code>textHeight</code> property affects a field only when the field’s <code>fixedLineHeight</code> property is true. 


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
