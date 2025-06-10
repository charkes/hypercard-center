---
title: selectedButton
card_id: 103123
---

# selectedButton

<code><pre>
the selectedButton of ¬
 [background | card] family [ph:intExpr]
</pre></code>

Value returned: the domain and number (for example,<code> card button 3</code>) of the highlighted button in the specified button family on the current card or background

If you don't specify <code>card</code> (or <code>cd</code>)<code></code> or <code>background</code> (or <code>bg</code> or<code> bkgnd</code>), the family is assumed to be on the card layer. 

If no button in the specified family is highlighted, <code>selectedButton </code>returns<code> empty</code>.

If the specified family doesn't exist, you get an error dialog box. 


## Examples

```


get the selectedButton of family 6 -- a card family

put the selectedButton of bg family 4 into hit
```

## Related Topics

* [family](/HyperTalkReference/properties/family)
