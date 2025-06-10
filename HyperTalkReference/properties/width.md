---
title: width
card_id: 89143
---

# width

<code>set </code>[<code>the</code>]<code> width of [ph:button] to [ph:integer] set </code>[<code>the</code>]<code> width of [ph:field] to [ph:integer]<u> </u>set </code>[<code>the</code>]<code> width of [ph:card] to [ph:integer] set </code>[<code>the</code>]<code> width of [ph:window] to integer get </code>[<code>the</code>]<code> width of menuBar <u> </code></u>The <code>width</code> property returns or sets an integer equal to the width in pixels of the specified object or window. Setting the width of a button, field, or card window resizes it. 

Setting the width of a card resizes all the cards in a stack. 

You can't set the menu bar's width. 


Note: HyperCard restricts the width of a card to 32-pixel increments beginning from 64, the smallest width. For example, setting the width of a card to 420 results in a width of 416.

HyperCard maintains the location (center coordinate) of the object, expanding or shrinking it on both
sides evenly.

## Examples

```
the width of card button 1
the width of bkgnd field id 34
the width of this card
the width of message box
the width of tool window
the width of card window

set the width of bkgnd button "Next" to the width of bg btn "Prev"
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
