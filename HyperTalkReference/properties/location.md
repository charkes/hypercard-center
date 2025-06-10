---
title: location
card_id: 74795
---

# location

<code>set </code>[<code>the</code>]<code> loc of [ph:button] to [ph:point] set </code>[<code>the</code>]<code> loc of [ph:field] to [ph:point] set </code>[<code>the</code>]<code> loc of [ph:window] to [ph:point] set </code>[<code>the</code>]<code> loc of [ph:externalWindow] ¬     to [ph:point] </code> The <code>location</code> (or<code> loc</code>) property returns or sets the <u>center</u> point of a button or field and the <u>top-left </u>corner of a window. Setting the location of button, field, or window moves it to the new location. 

HyperCard determines the location
of buttons, fields, and HyperCard’s built-in windows relative to the 
top-left corner of the current card. 

For a window displaying a stack, HyperCard determines the location of the card window relative to the top-left corner of the screen with the menu bar.

HyperCard adjusts the horizontal offset of the card window to the closest multiple of 16 to the number specified.

## Examples

```
the location of card button 1
the loc of bkgnd field id 34
set the loc of bkgnd button "Next" to the clickLoc

the loc of card window

-- built-in windows:
the loc of message box
the loc of tool window

-- external windows:
set the loc of window "Script of stack My HD:Home" to 100,100
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [screenRect](/HyperTalkReference/functions/screenRect)
* [scroll](/HyperTalkReference/properties/scroll)
* [show](/HyperTalkReference/commands/show)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
