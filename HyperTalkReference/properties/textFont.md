---
title: textFont
card_id: 84911
---

# textFont

<code>set </code>[<code>the</code>]<code> textFont to [ph:text</code>] <code>set </code>[<code>the</code>] <code>textFont of</code> [[ph:<code>chunk] of</code>]<code> ¬     [ph:field] to [ph:text] set </code>[<code>the</code>]<code> textFont of [ph:button] to [ph:text ]set </code>[<code>the</code>]<code> textFont of the message box¬                 to [ph:text] </code> where <code>[ph:text]</code> is the name of a font available from the current stack.

The <code>textFont</code> property returns or sets the current font of the Paint Text tool,  text in a field,  a button name, or the Message box. 

The default value is <code>Geneva</code> for fields,  Paint text, and the Message box; the default value is <code>Chicago</code> for buttons.

<b>Note</b>: if a chunk of a field contains a mixture of fonts, HyperCard returns <code>mixed</code> when you ask for<code> the textFont</code>. 


## Examples

```
the textFont of field 1
the textFont of the clickChunk
the textFont of the foundChunk

if the textFont of the clickChunk is "Monaco" then ...

set the textFont to "Geneva" -- for the text tool
set the textFont of field 1 to "New York"
set the textFont of card button 1 to "Geneva"
set the textFont of char 1 to 19 of line 2 of field 3 to "Monaco"
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
* [textAlign](/HyperTalkReference/properties/textAlign)
* [textHeight](/HyperTalkReference/properties/textHeight)
* [textSize](/HyperTalkReference/properties/textSize)
* [textStyle](/HyperTalkReference/properties/textStyle)
