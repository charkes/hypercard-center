---
title: autoHilite
card_id: 67503
---

# autoHilite

<code> set </code>[<code>the</code>]<code> autoHilite of [ph:button] ¬     to [ph:trueOrFalse] 

</code>The <code>autoHilite</code> property sets or returns whether a button highlights automatically in response to a <code>mouseDown</code> event.  

With check boxes and radio buttons, <code>autoHilite</code> determines whether the button can change from deselected to selected and vice versa. 

 The <code>autoHilite</code> property corresponds to the Auto Hilite check box in a Button Info dialog box.

Automatic highlighting occurs if <code> autoHilite </code>is set to<code> true</code>. 


## Examples

```
set the autoHilite of bkgnd button 1 to true

get the autoHilite of card button id 37
set the autoHilite of card button id 37 to not it
```

## Related Topics

* [hilite](/HyperTalkReference/properties/hilite)
* [sharedHilite](/HyperTalkReference/properties/sharedHilite)
