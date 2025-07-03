---
title: screenRect
card_id: 62877
---

# screenRect

```
the screenRect
```

Value returned: a `[ph:rectangle]` equal to the dimensions of the screen in pixels

If there's more than one monitor, `the screenRect` returns the dimensions of the monitor displaying the current stack as offsets from the top-left corner of the screen that contains the menu bar.

If the card window appears on more than one monitor, `the screenRect` returns the dimensions of the screen that shows the most area from the  card window. 

## Examples

```
get the screenRect
if the mouseLoc is not within it then ...

if the screenRect = "0,0,512,342" then ... -- SE size monitor
```

## Demo Script

```
on screenRectDemo
  get the <b>screenRect</b>
  put "The dimensions of the monitor displaying this stack are:" &¬
  return & return & "Width:" && (item 3 of it - item 1 of it) &¬
  return & "Height:" && (item 4 of it - item 2 of it) into sayIt
  answer sayIt
end screenRectDemo
```

## Related Topics

* [bottom](/HyperTalkReference/properties/bottom)
* [bottomRight](/HyperTalkReference/properties/bottomRight)
* [height](/HyperTalkReference/properties/height)
* [left](/HyperTalkReference/properties/left)
* [location](/HyperTalkReference/properties/location)
* [rectangle](/HyperTalkReference/properties/rectangle)
* [right](/HyperTalkReference/properties/right)
* [scroll](/HyperTalkReference/properties/scroll)
* [top](/HyperTalkReference/properties/top)
* [topLeft](/HyperTalkReference/properties/topLeft)
* [width](/HyperTalkReference/properties/width)
