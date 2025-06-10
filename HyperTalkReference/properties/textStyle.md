---
title: textStyle
card_id: 86415
---

# textStyle

<code> set </code>[<code>the</code>]<code> textStyle to [ph:textStyleList</code>] <code>set </code>[<code>the</code>] <code>textStyle of</code> [[ph:<code>chunk] of</code>]<code> ¬     [ph:field] to [ph:textStyleList] set </code>[<code>the</code>]<code> textStyle of [ph:button] ¬     to [ph:textStyleList] set the textStyle of [ph:menuItem] ¬     of [ph:menu] to [ph:textStyleList] set </code>[<code>the</code>]<code> textStyle of ¬ the message box to [ph:textStyleList ] </code>The <code>textStyle</code> property returns or sets the styles in which Paint text, field text, button names, menu items, or text in the Message box appear. 

 The style can be a single text style or a comma-separated list of styles. The available styles are<code> plain</code>,<code> bold</code>,<code> italic</code>,<code> underline</code>,<code> outline</code>,<code> shadow</code>,<code> condense</code>,<code> extend</code>, and<code> group</code>. (To see group text, issue the command<code> show groups.</code>)

The default text style is<code> plain</code>.

<b>Note</b>: if a chunk of a field contains a mixture of styles, HyperCard returns <code>mixed</code> when you ask for<code> the textStyle</code>. 


## Examples

```
the textStyle of field 1
the textStyle of the clickChunk
the textStyle of the foundChunk

if the textStyle of the clickChunk contains "group" then ...

if the textStyle of the clickChunk contains "bold" then ...

set the textStyle to 10 -- for the text tool
set the textStyle of field 1 to plain
set the textStyle of card button 1 to bold
set the textStyle of char 1 to 19 of line 2 of field 3 to bold,italic
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
* [show](/HyperTalkReference/commands/show)
* [textAlign](/HyperTalkReference/properties/textAlign)
* [textFont](/HyperTalkReference/properties/textFont)
* [textHeight](/HyperTalkReference/properties/textHeight)
* [textSize](/HyperTalkReference/properties/textSize)
