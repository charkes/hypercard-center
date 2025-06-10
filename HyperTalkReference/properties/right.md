---
title: right
card_id: 86116
---

# right

<code><pre>
the right of [ph:card]<u>
</u>
set
</pre></code>

[<code>the
</pre></code>

]<code> right of [ph:button] to [ph:integer] set </code>[<code>the</code>]<code> right of [ph:field] to [ph:integer] set </code>[<code>the</code>]<code> right of [ph:window] to [ph:integer]<u> </u>get </code>[<code>the</code>]<code> right of menuBar <u> </code></u>The <code>right</code> property returns or sets an integer equal to item 3 of an element’s rectangle.  If you set the right of an object, it moves horizontally; the object's size remains the same. You can’t set <code>the right</code> of cards: use the<code> rect</code>,<code> height</code>, or<code> width</code> properties to resize the cards in a stack. 

You can't set <code>the right</code> of the menu bar.

HyperCard determines<code> the right </code>of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the  current card. 

HyperCard determines <code>the right</code> of the card window relative to the top-left corner of the screen with the menu bar. 


## Examples

```
the right of card button 1
the right of bkgnd field id 34
the right of this card
the right of message box
the right of tool window
the right of card window

set the right of bkgnd button "Next" to the right of bg btn "Prev"
```

## Demo Script

<code><pre>
on moveButton
  put the <b>right </b>of bkgnd btn "Run the Script" into savedRight
  set cursor to none
  repeat for 23
    put the <b>right </b>of bkgnd btn "Run the Script" - 26 into newRight
    set the <b>right </b>of bkgnd btn "Run the Script" to newRight
    if the <b>right </b>of bkgnd btn "Run the Script" < 0
    then set the left of bkgnd btn "Run the Script" to ¬
    the width of card window
  end repeat
  set the <b>right </b>of bkgnd btn "Run the Script" to savedRight
end moveButton
</pre></code>

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
