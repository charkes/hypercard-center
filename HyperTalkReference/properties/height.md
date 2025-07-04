---
title: height
card_id: 86710
---

# height

` set `[`the`]` height of [ph:button] to [ph:integer] set `[`the`]<code> height of [ph:field] to [ph:integer]<u> </u>set </code>[`the`]` height of [ph:card] to [ph:integer] set `[`the`]<code> height of [ph:window] to [ph:integer]<u> </u>get </code>[`the`]` height of menuBar ` The `height` property returns or sets an integer equal to the height in pixels of an object or window. Setting the height of a button, field, or window resizes it. HyperCard maintains the location (center coordinate) of the object, expanding or shrinking it on both sides evenly. 

 Setting the height of a card resizes <u>all</u> the cards in a stack. HyperCard forces the integer specifying the height to be an even number greater than 64 pixels.

You can't set the height of the menu bar. 


## Examples

```
the height of card button 1
the height of bkgnd field id 34
the height of this card
the height of message box
the height of tool window
the height of card window

set the height of bkgnd button "Next" to the height of bg btn "Prev"
```

## Demo Script

```
on growAndShrinkButton
  repeat 15
    set <b>height</b> of bkgnd btn "Run the Script" to ¬
    (the <b>height</b> of bkgnd btn "Run the Script") + 2
    wait 1
  end repeat
  repeat 15
    set <b>height</b> of bkgnd btn "Run the Script" to ¬
    (the <b>height</b> of bkgnd btn "Run the Script") - 2
    wait 1
  end repeat
end growAndShrinkButton
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
