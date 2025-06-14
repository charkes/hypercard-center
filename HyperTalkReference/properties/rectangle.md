---
title: rectangle
card_id: 79936
modified: yes
---

# rectangle

<code><pre>
set [the] rect of <i>button</i> to <i>rectangle</i>
set [the] rect of <i>field</i> to <i>rectangle</i>
set [the] rect of <i>card</i> to <i>rectangle</i>
set [the] rect of <i>window</i> to <i>rectangle</i>
get [the] rect of menuBar
</pre></code>


The <code>rectangle</code> property returns or sets the rectangular coordinates of buttons, fields, cards, and windows, and it returns the coordinates of the menu bar. Setting the rectangle of a card changes the size of <u>all the cards</u> in a stack; setting the rectangle of the card window resizes the window, not the card.

HyperCard determines <code>the rectangle</code> of buttons, fields, cards, and its built-in windows relative to the top-left corner of the current card. HyperCard determines <code>the rectangle</code> of the card window relative to the top-left corner of the screen with the menu bar.

Note: You can’t set the <code>rect</code> of an inactive card window or of the menu bar.

## Examples

```
the rectangle of card button 1
the rectangle of bkgnd field id 34
the rectangle of this card
the rect of message box
the rect of tool window
the rect of card window

set the rect of bkgnd button "Next" to the rect of bg btn "Prev"

set the rect of card window to the rect of this card
```

## Demo Script

<code><pre>
on talkAboutRects
  answer "The rect of bkgnd btn “Run the Script” is:" && ¬
  the <b>rect</b> of bkgnd btn "Run the Script" & return & return & ¬
  "The rect of this card is:" && the <b>rect</b> of this card & return & ¬
  return &"The rect of the card window is:" && the <b>rect</b> of the card window
end talkAboutRects
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/rectangle.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/window.md]

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
