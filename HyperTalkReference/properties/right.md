---
title: right
card_id: 86116
---

# right

```
the right of [ph:card]<u>
</u>
set
```

[<code>the
```

]` right of [ph:button] to [ph:integer] set `[`the`]` right of [ph:field] to [ph:integer] set `[`the`]<code> right of [ph:window] to [ph:integer]<u> </u>get </code>[`the`]<code> right of menuBar <u> </code></u>The `right` property returns or sets an integer equal to item 3 of an element’s rectangle.  If you set the right of an object, it moves horizontally; the object's size remains the same. You can’t set `the right` of cards: use the` rect`,` height`, or` width` properties to resize the cards in a stack. 

You can't set `the right` of the menu bar.

HyperCard determines` the right `of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the  current card. 

HyperCard determines `the right` of the card window relative to the top-left corner of the screen with the menu bar. 


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

```
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
```

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
