---
title: textFont
card_id: 84911
---

# textFont

```
set [the] textFont to [ph:text]
set [the] textFont of [[ph:chunk] of] [ph:field] to [ph:text]
set [the] textFont of [ph:button] to [ph:text]
set [the] textFont of the message box to [ph:text]
```
where `[ph:text]` is the name of a font available from the current stack.

The `textFont` property returns or sets the current font of the Paint Text tool,  text in a field,  a button name, or the Message box.

The default value is `Geneva` for fields,  Paint text, and the Message box; the default value is `Chicago` for buttons.

<b>Note</b>: if a chunk of a field contains a mixture of fonts, HyperCard returns `mixed` when you ask for `the textFont`. 

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
