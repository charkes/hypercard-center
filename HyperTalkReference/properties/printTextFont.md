---
title: printTextFont
card_id: 90961
---

# printTextFont

<code><pre>
set the printTextFont to [ph:font]<u>
</pre></code>

</u>The <code>printTextFont</code> property returns or sets the value of the default text font used by the <code>print</code> command. The default value is<code> Geneva</code>.

When you print a report, HyperCard determines the default font for a report item as follows:

• If the report item is the text of a card     or  background field, HyperCard uses     the text font of the field. 

• If the report item is generated from     any other HyperTalk expression,     HyperCard uses the value of    <code> printTextFont</code>.

In either case, the user can override the default font by selecting a font in the Item Info dialog box of the report item. 


## Examples

```
set the printTextFont to "Times"
```

## Related Topics

* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
