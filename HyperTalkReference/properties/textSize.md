---
title: textSize
card_id: 85825
---

# textSize

<code> set </code>[<code>the</code>]<code> textSize to [ph:posInteger</code>] <code>set </code>[<code>the</code>] <code>textSize of</code> [[ph:<code>chunk] of</code>]<code> ¬     [ph:field] to [ph:posInteger] set </code>[<code>the</code>]<code> textSize of [ph:button] ¬     to [ph:posInteger] set </code>[<code>the</code>]<code> textSize of the message box¬                    to [ph:posInteger]

</code>The <code>textSize</code> property returns or sets the size, in pixels, of the font for Paint text, text in a field, a button name, or the Message box. The default value is 12. 

 <b>Note</b>: if a chunk of a field contains a mixture of sizes, HyperCard returns <code>mixed</code> when you ask for<code> the textSize</code>. 


## Examples

```
the textSize of field 1
the textSize of the clickChunk
the textSize of the foundChunk

if the textSize of the clickChunk is 10 then ...

set the textSize to 10 -- for the text tool
set the textSize of field 1 to 12
set the textSize of card button 1 to 9
set the textSize of char 1 to 19 of line 2 of field 3 to 24
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
* [textAlign](/HyperTalkReference/properties/textAlign)
* [textFont](/HyperTalkReference/properties/textFont)
* [textHeight](/HyperTalkReference/properties/textHeight)
* [textStyle](/HyperTalkReference/properties/textStyle)
