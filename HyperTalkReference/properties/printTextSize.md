---
title: printTextSize
card_id: 91932
---

# printTextSize

```
set the printTextSize to [ph:posInteger]
```

The `printTextSize` property returns or sets the value of the default text size (or point size) used by the `print` command. The default value is `10`.

When you print a report, HyperCard determines the default text size for a report item as follows:

* If the report item is the text of a card or background field, HyperCard uses the text size of the field.

* If the report item is generated from any other HyperTalk expression, HyperCard uses the value of the `printTextSize`.

In either case, the user can override the default size by selecting a size in the Item Info dialog box of the report item. 

## Examples

```
set the printTextSize to 18
```

## Related Topics

* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
* [reset](/HyperTalkReference/commands/reset)
