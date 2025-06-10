---
title: autoTab
card_id: 76921
---

# autoTab

<code> set </code>[<code>the</code>]<code> autoTab of [ph:field] to ¬     [ph:trueOrFalse]

</code>The <code>autoTab</code> property returns or sets whether HyperCard inserts a return character when the insertion point is on the last line of a field (<code>autoTab </code>is false) or moves the insertion point to the next editable field on the card (<code>autoTab </code>is true). 

Note: Auto tabbing doesn't work with scrolling fields. 

 The <code>autoTab</code> property corresponds to the Auto Tab check box in a Field Info dialog box. 


## Examples

```
set autoTab of card field 3 to true
set autoTab of field "address" to false
```

## Related Topics

* [returnKey](/HyperTalkReference/commands/returnKey)
* [tabKey](/HyperTalkReference/commands/tabKey)
