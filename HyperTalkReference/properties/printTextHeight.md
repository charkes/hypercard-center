---
title: printTextHeight
card_id: 91426
---

# printTextHeight

```
set the printTextHeight ¬
   to [ph:posInteger]<u>
```

</u>The `printTextHeight` property returns or sets the value of the default text height (or line spacing) used by the `print` command. The default value is `13`.

When you print a report, HyperCard determines the default text height for a report item as follows: 

• If the report item is the text of a card     or  background field, HyperCard uses     the text height of the field.

• If the report item is generated from     any other HyperTalk expression,     HyperCard uses the value of    ` printTextHeight`.

In either case, the user can override the default height by selecting a height in the Item Info dialog box of the report item. 


## Examples

```
set the printTextHeight to 20
```

## Related Topics

* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
* [reset](/HyperTalkReference/commands/reset)
