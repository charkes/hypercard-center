---
title: bottom
card_id: 85301
---

# bottom

```
the bottom of [ph:card]<u>
</u>
set
```

[<code>the
```

]` bottom of [ph:button] to [ph:integer] set `[`the`]` bottom of [ph:field] to [ph:integer] set `[`the`]<code> bottom of [ph:window] to [ph:integer]<u> </u>get </code>[`the`]` bottom of menuBar ` The `bottom` property returns or sets an integer equal to item 4 of an element’s rectangle. If you set the bottom of an element, it moves vertically; its size remains the same. You can’t set the `bottom` of cards: use the` rect`,` height`, and` width` properties to resize the cards in a stack. 

You can’t set the `bottom` of  the menu bar.

HyperCard determines the` bottom `of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the current card. 

HyperCard determines the `bottom` of the card window relative to the top-left corner of the screen with the menu bar. 


## Examples

```
the bottom of card button 1
the bottom of bkgnd field id 34
the bottom of this card
the bottom of message box
the bottom of tool window
the bottom of card window

set the bottom of bkgnd button "Next" to the bottom of bg btn "Prev"
```

## Related Topics

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
* [width](/HyperTalkReference/properties/width)
