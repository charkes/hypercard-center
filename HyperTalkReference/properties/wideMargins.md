---
title: wideMargins
card_id: 88854
---

# wideMargins

<code> set </code>[<code>the</code>]<code> wideMargins of [ph:field] ¬     to [ph:trueOrFalse]

</code>The <code>wideMargins</code> property returns or sets whether HyperCard adds extra space between the edges of a field and its text (to make it easier to read). It corresponds to the Wide Margins check box in a Field Info dialog box.

The default value is false. 


## Examples

```
set the wideMargins of bkgnd field 2 to true
```

## Demo Script

<code><pre>
on wideMarginsDemo
  set the wideMargins of me to false
  wait 2 seconds
  set the wideMargins of me to true
end wideMarginsDemo
</pre></code>

## Related Topics

* [style](/HyperTalkReference/properties/style)
