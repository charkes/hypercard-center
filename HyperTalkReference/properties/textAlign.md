---
title: textAlign
card_id: 83738
---

# textAlign

<code> set </code>[<code>the</code>]<code> textAlign to [ph:alignment] set </code>[<code>the</code>]<code> textAlign of [ph:field] ¬     to [ph:alignment] set </code>[<code>the</code>]<code> textAlign of [ph:button] ¬     to [ph:alignment]

</code>The <code>textAlign</code> property returns or sets the way Paint text, text in a field, or a button name aligns within its rectangle. It can align <code>left</code>, <code>right</code>, or<code> center</code>. The default value is<code> left</code> for fields and paint text, and <code>center</code> for buttons. 

 You can set the <code>textAlign</code> for radio buttons and check boxes, but the text always displays aligned <code>left</code>. 

You can’t set the <code>textAlign</code> for a  chunk of text. 


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
