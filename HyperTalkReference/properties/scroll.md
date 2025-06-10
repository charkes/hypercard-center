---
title: scroll
card_id: 81344
---

# scroll

<code>set </code>[<code>the</code>]<code> scroll of [ph:field] to [ph:integer] set the scroll of </code>[<code>the</code>]<code> card window ¬     to [ph:point</code>]

For scrolling fields, the <code>scroll</code> property returns or sets which lines of text currently appear (as indicated by the scroll bar). The <code>[ph:integer]</code> represents the number of pixels that have scrolled above the top of the field’s rectangle. For example, the number of lines scrolled in card field 1 equals<code> the scroll of card field 1 div the textHeight of card field 1</code>. 

For fields, HyperCard pins the <code>scroll</code> to a number between 0 and the maximum value for the field.

For the card window, the <code>scroll</code> property returns or sets a point that specifies the current horizontal and vertical offsets of the portion of the card currently visible in the card window. It affects the card image only when the size of the window is smaller than the size of the card. 


## Examples

```
if the textHeight of field "index" is 18 then
set scroll of field "index" to 36

scrolls down by two lines.

put the scroll of field 1 div textHeight of field 1 into linesScrolled
set the scroll of field "Index" to 0

set the scroll of the card window to 0,0
set the scroll of card window to (bottomRight of this card)
```

## Demo Script

<code><pre>
on madScroller
  put the rect of card window into theRect
  set the rect of card window to left of cd window,top of cd window,¬
  left of cd window + 172, top of cd window + 64
  repeat 10 times
    set the <b>scroll</b> of card window to ¬
    random(width of this card),random(height of this card)
    wait 30
  end repeat
  set the rect of card window to theRect
end madScroller
</pre></code>

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [style](/HyperTalkReference/properties/style)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
