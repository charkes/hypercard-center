---
title: grid
card_id: 72386
---

# grid

<code> set </code>[<code>the</code>]<code> grid to [ph:trueOrFalse]

</code>The <code>grid</code> property returns or sets whether HyperCard constrains the movement of many Paint tools to eight-pixel intervals. It corresponds to the Grid command in the Options menu (which appears when you select a Paint tool).

The default value is<code> false</code>. 


## Examples

```
set the grid to true
```

## Demo Script

<code><pre>
on gridDemo
  setUpPaint
  show bkgnd field "demo field"
  displayMessage "Click the mouse to continue..." & return &¬
  "Grid set to false" & spaces(30) & "Grid set to true"
  set <b>grid</b> to false
  set dragspeed to 200
  drag from "20,110" to "165,250"
  wait 2 seconds
  set <b>grid</b> to true
  drag from "265,110" to "410,250"
  set the cursor to arrow
  wait until the mouseClick
  domenu "revert"
  hide bkgnd field "demo field"
  choose browse tool
end gridDemo

on setUpPaint
  choose rectangle tool
  set lineSize to 1
  set multiple to true
  set polysides to 4
  show card picture
  set centered to false
  set filled to false
end setUpPaint
</pre></code>

## Related Topics

* [reset](/HyperTalkReference/commands/reset)
