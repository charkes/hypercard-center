---
title: fixedLineHeight
card_id: 71811
---

# fixedLineHeight

```
set [the] fixedLineHeight of [ph:field] ¬
     to [ph:trueOrFalse]
```

The `fixedLineHeight` property returns or sets whether a field has uniform line height or varies the line height of each line according to largest font size that appears in the line.

It corresponds to the Fixed Line Height check box in a Field Info dialog box.

Setting the `fixedLineHeight` property to `false` sets the `showLines` property to `false`. Setting `the fixedLineHeight` to `true` has no effect on `the showLines`. 

## Examples

```
set the fixedLineHeight of bkgnd field id 24 to false
```

## Related Topics

* [showLines](/HyperTalkReference/properties/showLines)
* [style](/HyperTalkReference/properties/style)
