---
title: left
card_id: 74022
modified: yes
---

# left

<code><pre>
the left of <i>card</i>
set [the] left of <i>button</i> to <i>integer</i>
set [the] left of <i>field</i> to <i>integer</i>
set [the] left of <i>window</i> to <i>integer</i>
get [the] left of menuBar
</pre></code>


The<code> left </code>property returns or sets an integer equal to item 1 of an object’s rectangle. If you set the<code> left </code>of an object, it moves horizontally. The size of the object remains the same. You can’t set the<code> left </code>of cards: use the<code> rect</code>,<code> height</code>, and<code> width</code> properties to resize the cards in a stack.

You can't set the<code> left </code>of the menu bar.

HyperCard determines the<code> left </code>of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the current card.

HyperCard determines the<code> left </code>of the card window relative to the top-left corner of the screen with the menu bar.

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

## Placeholders

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/integer.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/window.md]

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
