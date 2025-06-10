---
title: bottomRight
card_id: 91818
---

# bottomRight

<code><pre>
the bottomRight of [ph:card]<u>
</u>
set
</pre></code>

[<code>the
</pre></code>

]<code> bottomRight of [ph:button] ¬     to [ph:point] set </code>[<code>the</code>]<code> bottomRight of [ph:field] ¬     to [ph:point] get </code>[<code>the</code>]<code> bottomRight of menuBar <u> </code></u>The <code>bottomRight</code> property returns or sets a <code>[ph:point]</code> equal to items 3 and 4 of an element’s rectangle. If you set the <code>bottomRight</code> of an element, it moves; the element's size remains the same. 

You can’t set the <code>bottomRight</code> of cards: use the<code> rect</code>,<code> height</code>, and<code> width</code> properties to resize the cards in a stack.

HyperCard determines the <code>bottomRight </code> of buttons, fields, and  built-in windows relative to the top-left corner of the current card.  It determines the<code> bottomRight</code> of the card window relative to the top-left corner of the screen with the menu bar. 


## Examples

```
the bottomRight of card button 1
the bottomRight of bkgnd field id 34
the bottomRight of this card
the botRight of card window

set the botRight of bkgnd button "Next" to the botRight of bg btn "Prev"
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
