---
title: selectedLine
card_id: 63809
modified: yes
---

# selectedLine

<code><pre>
the selectedLine
the selectedLine of <i>listField</i>
the selectedLine of <i>popupButton</i>
</pre></code>


Values returned:

* for<code> the selectedLine</code>, a line     expression that indicates the line of a     field or the Message box in which a     range of characters is currently     highlighted

* for<code> the selectedLine of <i>listField, </i></code>    a line expression that indicates the     lines of a <i>list field</i>  in which the     characters are currently highlighted

* for<code> the selectedLine of</code> <i><code>popupButton</i></code>,     a line expression that evaluates to      the line number in a popup button’s     contents indicating the current     selection

If nothing is selected, <code>the selectedLine</code> returns <code>empty</code>.

If a field isn't currently a list field but  it was in the past, and a selection had been made when it was a list field, <code>the selectedLine</code> returns the most recent selection.

The line expression returned has the following forms:

<code><pre>
line <i>i</i> of {card|bkgnd} field <i>n</i>
line <i>i </i>of {card|bkgnd} button <i>n</i>
line <i>x</i> to <i>y</i> of {card|bkgnd} field <i>n</i>
</pre></code>


where<code> <i>i</i> </code>is the line number and <i><code>n</i> </code>is the number of a popup button or a  field, and<code> <i>x</i> to <i>y</i> </code>is a range of lines in a <i>list field</i>.

## Examples

```
get the selectedLine

put the selectedLine into theLine
set the textFont of theLine to "Geneva"

get the selectedLine of button "My Popup Button"
get the selectedLine of field "My List Field"
```

## Placeholders

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
* [clickLine](/HyperTalkReference/functions/clickLine)
* [foundLine](/HyperTalkReference/functions/foundLine)
* [select](/HyperTalkReference/commands/select)
