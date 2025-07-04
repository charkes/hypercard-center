---
title: sharedText
card_id: 82124
---

# sharedText

`set `[`the`]` sharedText of [ph:field] ¬     to [ph:trueOrFalse] ` where `[ph:field]` is a background field only.

The `sharedText` property returns or sets whether a background field displays the same text on every card of the background. The default value for new fields is false, meaning the text in the field can be different on each card. 

Set `sharedText` to true if you want the same text to appear on each card of the background. To enter text into a background field with `sharedText` set to true, choose Background from the Edit menu, and type in the field. You can  add shared text only while you’re in the background layer.

HyperCard does <u>not</u> discard either card-specific text or shared text—it will display the appropriate text when you set the `sharedText` to true or false. 


## Examples

```
set the sharedText of bkgnd field 1 to true
```

