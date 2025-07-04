---
title: family
card_id: 99648
---

# family

```
set [the] family of [ph:button] to [ph:integer]
```

where `[ph:integer]` resolves to a value between 0 and 15, and 0 means “no family.”

This property sets or retrieves the button family for a given button.

Setting the hilite of any button in a family to `true` sets the hilite of all other same-family buttons to `false`.

The default `family` value for a new button is 0.

Card and button families are distinct; so there can be a family [ph:n ] for card buttons and another family [ph:n ] for background buttons.  

You can also assign a button to a family by using the Family pop-up menu in the button's Get Info dialog box.

## Examples

```
set family of background button "moo" to 3

if the family of button 3 is targetFamily then go stack farmAnimal
```

## Related Topics

* [selectedButton](/HyperTalkReference/functions/selectedButton)
* [sharedHilite](/HyperTalkReference/properties/sharedHilite)
