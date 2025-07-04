---
title: printTextStyle
card_id: 92736
---

# printTextStyle

```
set the printTextStyle to [ph:textStyleList]
```

The `printTextStyle` property returns or sets the value of the default text style used by the `print` command when you print an expression. The default value is `plain`.

When you print a report, HyperCard determines the default text style for a report item as follows:

* If the report item is the text of a card or background field, HyperCard uses the text style of the field.

* If the report item is generated from any other HyperTalk expression, HyperCard uses the value of the `printTextStyle`.

In either case, the user can override the default style by selecting a style in the Item Info dialog box of the report item.

## Examples

```
set the printTextStyle to "bold"
set the printTextStyle to "bold,italic"
```

## Related Topics

* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [reset](/HyperTalkReference/commands/reset)
