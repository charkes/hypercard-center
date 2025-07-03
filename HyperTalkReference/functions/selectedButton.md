---
title: selectedButton
card_id: 103123
---

# selectedButton

```
the selectedButton of ¬
 [background | card] family [ph:intExpr]
```

Value returned: the domain and number (for example, `card button 3`) of the highlighted button in the specified button family on the current card or background

If you don't specify `card` (or `cd`) or `background` (or `bg` or `bkgnd`), the family is assumed to be on the card layer.

If no button in the specified family is highlighted, `selectedButton` returns `empty`.

If the specified family doesn't exist, you get an error dialog box.

## Examples

```
get the selectedButton of family 6 -- a card family

put the selectedButton of bg family 4 into hit
```

## Related Topics

* [family](/HyperTalkReference/properties/family)
