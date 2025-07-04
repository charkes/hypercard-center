---
title: autoTab
card_id: 76921
---

# autoTab

```
set [the] autoTab of [ph:field] to ¬
     [ph:trueOrFalse]
```

The `autoTab` property returns or sets whether HyperCard inserts a return character when the insertion point is on the last line of a field (`autoTab` is false) or moves the insertion point to the next editable field on the card (`autoTab` is true). 

Note: Auto tabbing doesn't work with scrolling fields.

The `autoTab` property corresponds to the Auto Tab check box in a Field Info dialog box.

## Examples

```
set autoTab of card field 3 to true
set autoTab of field "address" to false
```

## Related Topics

* [returnKey](/HyperTalkReference/commands/returnKey)
* [tabKey](/HyperTalkReference/commands/tabKey)
