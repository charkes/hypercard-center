---
title: polySides
card_id: 78788
---

# polySides

` set `[`the`]` polySides to [ph:posInteger] ` where `[ph:posInteger]` is 0 or a number from 3 to 50.

The `polySides` property returns or sets the number of sides of a polygon created by the Regular Polygon tool.  Set `polySides` to 0 to draw a circle.

(You can also select one of six standard polygons by choosing Polygon Sides from the Options menu.) 

 If you set `polySides` to a number lower than 3 (other than 0) or higher than 50, it automatically reverts to 3 or 50. 


## Examples

```
set the polySides to 0 -- circle
set the polySides to 4
set the polySides to 28
```

## Demo Script

```
```
on polySidesDemo
 show bkgnd field "demo field"
 setUpPaint
 set dragspeed to 250
 put "50,16,12,10,9,8,7,6,5,4,3" into theSides
 repeat with itemNum = 1 to the number of items in theSides
   set <b>polysides</b> to (item itemNum of theSides)
   drag from "240,160" to "240,250"
 end repeat
 displayMessage "Click the mouse" & return & "to continue . . ."
 set the cursor to arrow
 wait until the mouseClick
 domenu "revert"
 hide bkgnd field "demo field"
 choose browse tool
end polySidesDemo
on setUpPaint
 show card picture
 set lineSize to 1
 choose regular polygon tool
 set the pattern to 1
 set centered to true
 set filled to true
 set grid to false
end setUpPaint
```
```

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
