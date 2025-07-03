---
title: clickH and clickV
card_id: 53066
---

# clickH and clickV

```
the clickH
the clickV
```

Values returned:

`clickH` returns an integer equal to the number of horizontal pixels from the left side of the card to the place the mouse was last clicked.

`clickV` returns an integer equal to the number of vertical pixels from the top of the card to the place the mouse was last clicked.

## Examples

```
click at 256,171
put the clickH  -- same as item 1 of the clickLoc
put the clickV  -- same as item 2 of the clickLoc

-- Use clickV to place the top of some buttons into alignment
-- based on the user’s click:
get the clickV
set the top of bkgnd button 1 to it
set the top of bkgnd button 2 to it
set the top of bkgnd button 3 to it
```

## Demo Script

```
on clickDemo
  show bkgnd field "demo field"
  displayMessage "Click the mouse to continue..."
  wait until the mouseClick
  answer "The horizontal point of the click was:" && the <b>clickH</b> && ¬
  return &"The vertical point of the click was:" && the <b>clickV</b>
  hide bkgnd field "demo field"
end clickDemo
```

## Related Topics

* [mouseH and mouseV](/HyperTalkReference/functions/mouseH-and-mouseV)
