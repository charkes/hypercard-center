---
title: selectedLine
card_id: 63809
modified: yes
---

# selectedLine

```
the selectedLine
the selectedLine of <i>listField</i>
the selectedLine of <i>popupButton</i>
```

Values returned:

* for `the selectedLine`, a line expression that indicates the line of a field or the Message box in which a range of characters is currently highlighted

* for `the selectedLine of [ph:listField]`, a line expression that indicates the     lines of a <i>list field</i> in which the characters are currently highlighted

* for `the selectedLine of [ph:popupButton]`, a line expression that evaluates to      the line number in a popup button’s contents indicating the current selection

If nothing is selected, `the selectedLine` returns `empty`.

If a field isn't currently a list field but it was in the past, and a selection had been made when it was a list field, `the selectedLine` returns the most recent selection.

The line expression returned has the following forms:

```
line <i>i</i> of {card|bkgnd} field <i>n</i>
line <i>i</i> of {card|bkgnd} button <i>n</i>
line <i>x</i> to <i>y</i> of {card|bkgnd} field <i>n</i>
```

where `[ph:i]` is the line number and `[ph:n]` is the number of a popup button or a  field, and `[ph:x]` to `[ph:y]` is a range of lines in a <i>list field</i>.

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
