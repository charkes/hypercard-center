---
title: selectedText
card_id: 64031
---

# selectedText

```
the selectedText
the selectedText of [ph:listField]
the selectedText of [ph:popupButton]
```

Value returned: a string equal to the range of characters currently selected.  If nothing is highlighted, it returns `empty`.

If a field isn't currently a list field but it was in the past, and a selection had been made when it was a list field, `the selectedText` returns the most recent selection.

## Demo Script

```
on whatIsTheSelection
  select line 2 of me
  answer "The selectText is “" & the selectedText & "”"
end whatIsTheSelection
```

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
* [clickText](/HyperTalkReference/functions/clickText)
* [foundText](/HyperTalkReference/functions/foundText)
* [select](/HyperTalkReference/commands/select)
