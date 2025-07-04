---
title: top
card_id: 86868
modified: yes
---

# top

```
the top of <i>card</i>
set [the] top of <i>button</i> to <i>Integer</i>
set [the] top of <i>field</i> to <i>Integer</i>
set [the] top of <i>window</i> to <i>Integer</i>
set [the] top of menuBar
```


The` top `property returns or sets an integer equal to item 2 of an element’s rectangle. If you set the top of an object, it moves vertically; the object's size remains the same. You can’t set` the top `of cards: use the` rect`,` height`, and` width` properties to resize the cards in a stack.

You can't set` the top `of the menu bar.

HyperCard determines` the top `of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the current card.

HyperCard determines` the top `of the card window relative to the top-left corner of the screen with the menu bar.

## Examples

```
the top of card button 1
the top of bkgnd field id 34
the top of this card
the top of message box
the top of tool window
the top of card window

set the top of bkgnd button "Next" to the top of bg btn "Prev"
```

## Placeholders

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/Integer.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/window.md]

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
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
