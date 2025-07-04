---
title: autoHilite
card_id: 67503
---

# autoHilite

```
set [the] autoHilite of [ph:button] ¬
     to [ph:trueOrFalse]
```

The `autoHilite` property sets or returns whether a button highlights automatically in response to a `mouseDown` event.  

With check boxes and radio buttons, `autoHilite` determines whether the button can change from deselected to selected and vice versa.

The `autoHilite` property corresponds to the Auto Hilite check box in a Button Info dialog box.

Automatic highlighting occurs if `autoHilite` is set to `true`. 

## Examples

```
set the autoHilite of bkgnd button 1 to true

get the autoHilite of card button id 37
set the autoHilite of card button id 37 to not it
```

## Related Topics

* [hilite](/HyperTalkReference/properties/hilite)
* [sharedHilite](/HyperTalkReference/properties/sharedHilite)
