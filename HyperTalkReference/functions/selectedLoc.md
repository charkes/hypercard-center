---
title: selectedLoc
card_id: 2765
---

# selectedLoc

<code><pre>
the selectedLoc
</pre></code>

Value returned: a <code>[ph:point]</code> equal to the left and bottom offsets of the insertion point or the current selection in a field

It returns <code>empty</code> if there is no selection or if the insertion point is in the Message box. 


## Examples

```
set the bottom of button "Hiliter" to item 2 of the selectedLoc
```

## Demo Script

<code><pre>
on whereIsTheSelection
  select word 2 of line 3 of me
  answer "The selectedLoc is" && the selectedLoc
end whereIsTheSelection
</pre></code>

## Related Topics

* [clickLoc](/HyperTalkReference/functions/clickLoc)
* [mouseLoc](/HyperTalkReference/functions/mouseLoc)
* [select](/HyperTalkReference/commands/select)
