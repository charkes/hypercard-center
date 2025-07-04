---
title: left
card_id: 74022
modified: yes
---

# left

```
the left of [ph:card]
set [the] left of [ph:button] to [ph:integer]
set [the] left of [ph:field] to [ph:integer]
set [the] left of [ph:window] to [ph:integer]
get [the] left of menuBar
```

The `left` property returns or sets an integer equal to item 1 of an object’s rectangle. If you set the `left` of an object, it moves horizontally. The size of the object remains the same. You can’t set the `left` of cards: use the `rect`, `height`, and `width` properties to resize the cards in a stack.

You can't set the `left` of the menu bar.

HyperCard determines the `left` of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the current card.

HyperCard determines the `left` of the card window relative to the top-left corner of the screen with the menu bar.

## Examples

```
the left of card button 1
the left of bkgnd field id 34
the left of this card
the left of message box
the left of tool window
the left of card window

set the left of bkgnd button "Next" to the left of bg btn "Prev"
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
