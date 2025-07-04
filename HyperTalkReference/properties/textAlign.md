---
title: textAlign
card_id: 83738
---

# textAlign

` set `[`the`]` textAlign to [ph:alignment] set `[`the`]` textAlign of [ph:field] ¬     to [ph:alignment] set `[`the`]<code> textAlign of [ph:button] ¬     to [ph:alignment]

</code>The `textAlign` property returns or sets the way Paint text, text in a field, or a button name aligns within its rectangle. It can align `left`, `right`, or` center`. The default value is` left` for fields and paint text, and `center` for buttons. 

 You can set the `textAlign` for radio buttons and check boxes, but the text always displays aligned `left`. 

You can’t set the `textAlign` for a  chunk of text. 


## Examples

```
set the textAlign to center -- for the text tool
set the textAlign of bkgnd field 2 to right
set the textAlign of button "Index" to left
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
* [textFont](/HyperTalkReference/properties/textFont)
* [textHeight](/HyperTalkReference/properties/textHeight)
* [textSize](/HyperTalkReference/properties/textSize)
* [textStyle](/HyperTalkReference/properties/textStyle)
