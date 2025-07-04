---
title: bottomRight
card_id: 91818
---

# bottomRight

```
the bottomRight of [ph:card]<u>
</u>
set
```

[<code>the
```

]` bottomRight of [ph:button] ¬     to [ph:point] set `[`the`]` bottomRight of [ph:field] ¬     to [ph:point] get `[`the`]<code> bottomRight of menuBar <u> </code></u>The `bottomRight` property returns or sets a `[ph:point]` equal to items 3 and 4 of an element’s rectangle. If you set the `bottomRight` of an element, it moves; the element's size remains the same. 

You can’t set the `bottomRight` of cards: use the` rect`,` height`, and` width` properties to resize the cards in a stack.

HyperCard determines the `bottomRight ` of buttons, fields, and  built-in windows relative to the top-left corner of the current card.  It determines the` bottomRight` of the card window relative to the top-left corner of the screen with the menu bar. 


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
