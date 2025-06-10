---
title: sharedHilite
card_id: 81699
---

# sharedHilite

<code> set </code>[<code>the</code>]<code> sharedHilite of [ph:button] ¬     to [ph:trueOrFalse] </code> where <code>[ph:button]</code> is a background button only.

The <code>sharedHilite</code> property returns or sets whether a background button shares its <code>hilite</code> property with every card in the background. The default value for new buttons is true. 

 Set <code>sharedHilite</code> to false if you want the <code>hilite</code> property for the background button maintained independently for each card.

For example, you might have one check box button in the background for marking and unmarking cards. You would set its <code>sharedHilite</code> to false so that its highlighting can be different on each card. 


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
