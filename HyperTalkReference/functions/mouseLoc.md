---
title: mouseLoc
card_id: 59412
---

# mouseLoc

```
the mouseLoc
```

Value returned: a `[ph:point]` equal to the current position of the mouse pointer relative to the current card


## Examples

```
get the mouseLoc
if it is within the rect of card button 1 then ...

set the loc of button 1 to mouseLoc()

if the mouseLoc is not within the rect of card window then beep
```

## Demo Script

```
on mouseLocDemo
 set the cursor to arrow
 show bkgnd field "demo field"
 put "Move the mouse to change the mouseLoc." & return & return &¬
 "The mouseLoc is:" && the <b>mouseLoc</b> into bkgnd field "demo field"
 put spaces(20) & "Click the mouse to stop . . ." into ¬
 line 5 of bkgnd field "demo field"
 repeat until the mouseClick
   put the <b>mouseLoc</b> into last word of line 3 of ¬
   bkgnd field "demo field"
 end repeat
 hide bkgnd field "demo field"
 put empty into bkgnd field "demo field"
end mouseLocDemo
```

## Related Topics

* [clickLoc](/HyperTalkReference/functions/clickLoc)
* [mouseH and mouseV](/HyperTalkReference/functions/mouseH-and-mouseV)
