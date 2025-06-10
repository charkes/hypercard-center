---
title: fixedLineHeight
card_id: 71811
---

# fixedLineHeight

<code> set </code>[<code>the</code>]<code> fixedLineHeight of [ph:field] ¬     to [ph:trueOrFalse</code>]

The <code>fixedLineHeight</code> property returns or sets whether a field has uniform line height or varies the line height of each line according to largest font size that appears in the line.

It corresponds to the Fixed Line Height check box in a Field Info dialog box. 

 Setting the <code>fixedLineHeight</code> property to <code> false</code> sets the <code>showLines </code>property to <code> false</code>. <code></code>Setting<code> the fixedLineHeight</code> to <code>true </code>has no effect on<code> the showLines</code>. 


## Examples

```
set the fixedLineHeight of bkgnd field id 24 to false
```

## Related Topics

* [showLines](/HyperTalkReference/properties/showLines)
* [style](/HyperTalkReference/properties/style)
