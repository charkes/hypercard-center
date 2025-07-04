---
title: dragSpeed
card_id: 70900
---

# dragSpeed

` set `[`the`]` dragSpeed to [ph:posInteger`]

The `dragSpeed` property returns or sets how many pixels per second the pointer will move when manipulated by all subsequent `drag` commands.  Use 0 to drag as fast as possible.

The `dragSpeed` affects all of the paint tools except the Bucket and Text tools.  

On idle, HyperCard resets the `dragSpeed` to 0. 


## Examples

```
set the dragSpeed to 0

set the dragSpeed to 100
```

## Demo Script

```
```
on dragSpeedDemo
 setUpPaint
 displayMessage "Drag speeds" & return & spaces(4) & "50" & ¬
 spaces(11) & "75" & spaces(11) & "150" & spaces(9) & "225" & ¬
 spaces(10) & "450" & spaces(10) & "800" & spaces(6) & "1600" & ¬
 spaces(8) & "2200" & spaces(9) & "0"
 set the textSize of line 2 of bkgnd field "Demo Field" to 14
 show bkgnd field "Demo Field"
 choose rect tool
 drawShape "16,230","59,105","50"
 drawShape "64,105","107,230","75"
 drawShape "113,230","156,105","150"
 drawShape "162,105","205,230","225"
 drawShape "211,230","254,105","450"
 drawShape "259,105","302,230","800"
 drawShape "308,230","351,105","1600"
 drawShape "357,105","400,230","2200"
 drawShape "405,230","448,105","0"
 wait 65
 domenu "revert"
 hide bkgnd field "Demo Field"
 choose browse tool
end dragSpeedDemo
on drawShape  startTopLeft, endBotRight, theDragSpeed
 set <b>dragSpeed</b> to theDragSpeed
 drag from startTopLeft to endBotRight
end drawShape
on setUpPaint
 show card picture
 set centered to FALSE
 set lineSize to 2
 set filled to FALSE
 set grid to FALSE
 set multiple to FALSE
end setUpPaint
```
```

## Related Topics

* [drag](/HyperTalkReference/commands/drag)
