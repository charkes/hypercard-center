---
title: style
card_id: 83265
---

# style

```
set [the] the style of [ph:button] to [ph:btnStyle]
set [the] the style of [ph:field] to [ph:fldStyle]
```

The `style` property returns or sets the style of button or field. It corresponds to the items in the Style pop-up menu in a Button Info or a Field Info dialog box.

A button can have one of the following styles: `transparent`, `opaque`, `rectangle`, `roundRect`, `checkBox`, `popup`, `oval`, `default`, `shadow`, `standard`, or `radioButton`.

A field can have one of the following styles: `transparent`, `opaque`, `rectangle`, `shadow`, or `scrolling`.

## Examples

```
set the style of bkgnd button 1 to rectangle
set the style of card field id 38 to shadow
```

## Related Topics

* [textAlign](/HyperTalkReference/properties/textAlign)
* [textFont](/HyperTalkReference/properties/textFont)
* [textHeight](/HyperTalkReference/properties/textHeight)
* [textSize](/HyperTalkReference/properties/textSize)
* [textStyle](/HyperTalkReference/properties/textStyle)
