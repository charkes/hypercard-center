---
title: selectedText
card_id: 64031
---

# selectedText

<code><pre>
the selectedText
the selectedText of [ph:listField]
the selectedText of [ph:popupButton]
</pre></code>

Value returned: a string equal to the range of characters currently selected.  If nothing is highlighted, it returns<code> empty</code>.

If a field isn't currently a list field but it was in the past, and a selection had been made when it was a list field, <code>the selectedText</code> returns the most recent selection. 


## Demo Script

<code><pre>
on whatIsTheSelection
  select line 2 of me
  answer "The selectText is “" & the selectedText & "”"
end whatIsTheSelection
</pre></code>

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
* [clickText](/HyperTalkReference/functions/clickText)
* [foundText](/HyperTalkReference/functions/foundText)
* [select](/HyperTalkReference/commands/select)
