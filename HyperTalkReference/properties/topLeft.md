---
title: topLeft
card_id: 87153
---

# topLeft

<code><pre>
the topLeft of [ph:card]<u>
</u>
set
</pre></code>

[<code>the
</pre></code>

]<code> topLeft of [ph:button] to [ph:point] set </code>[<code>the</code>]<code> topLeft of [ph:field] to [ph:point] set </code>[<code>the</code>]<code> topLeft of [ph:window] to [ph:point]<u> </u>get </code>[<code>the</code>]<code> topLeft of menuBar<u>

</code></u>The <code>topLeft</code> property returns or sets a <code>[ph:point]</code> equal to items 1 and 2 of an element’s rectangle. If you set <code>the topLeft</code> of an object, it moves; the object's size remains the same. You can’t set <code>the topLeft</code> of cards: use the<code> rect</code>,<code> height</code>, and<code> width</code> properties to resize the cards in a stack. 

You can’t set <code>the topLeft</code> of the menu bar.

HyperCard determines<code> the topLeft </code>of buttons, fields, and HyperCard’s built-in windows relative to the top-left corner of the current card. 

HyperCard determines <code>the topLeft</code> of the card window relative to the top-left corner of the screen with the menu bar. 


## Examples

```
the topLeft of card button 1
the topLeft of bkgnd field id 34
the topLeft of this card
the topLeft of message box
the topLeft of tool window
the topLeft of card window

set the topLeft of bkgnd button "Next" to the topLeft of bg btn "Prev"
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
* [width](/HyperTalkReference/properties/width)
