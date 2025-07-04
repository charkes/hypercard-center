---
title: sharedHilite
card_id: 81699
---

# sharedHilite

` set `[`the`]` sharedHilite of [ph:button] ¬     to [ph:trueOrFalse] ` where `[ph:button]` is a background button only.

The `sharedHilite` property returns or sets whether a background button shares its `hilite` property with every card in the background. The default value for new buttons is true. 

 Set `sharedHilite` to false if you want the `hilite` property for the background button maintained independently for each card.

For example, you might have one check box button in the background for marking and unmarking cards. You would set its `sharedHilite` to false so that its highlighting can be different on each card. 


## Examples

```
set the sharedHilite of bkgnd button 1 to true

get the sharedHilite of bkgnd button id 37
set the sharedHilite of bkgnd button id 37 to not it
```

## Related Topics

* [autoHilite](/HyperTalkReference/properties/autoHilite)
* [family](/HyperTalkReference/properties/family)
* [hilite](/HyperTalkReference/properties/hilite)
