---
title: drag
card_id: 35701
---

# drag

<code><pre>
drag from [ph:point] to [ph:point]
drag from [ph:point] to [ph:point] with [ph:key1]<u>
</u>drag from [ph:point] to [ph:point] ¬
  with [ph:key1], [ph:key2]<u>
</u>drag from [ph:point] to [ph:point] ¬
  with [ph:key1], [ph:key2], [ph:key3]<u>
</pre></code>

</u> The <code>drag</code> command simulates the user dragging the mouse manually (except that you must use the <code>with shiftKey</code> option in order to select text in a field). 

The <code>with [ph:key]</code> options specify combinations of the <code>commandKey</code>, the <code>optionKey</code>, and the <code>shiftKey</code>, simulating the user holding down the key or keys while dragging. 


## Examples

```
drag from 0,0 to 100,100
drag from 0,0 to 100,100 with shiftKey
drag from 0,0 to 100,100 with shiftKey,cmdKey,optionKey

drag from the mouseLoc to the bottomRight of this card
```

## Demo Script

<code><pre>
on mouseUp
  set the cantModify of this stack to true
  show bkgnd field "Demo Field"
  show card picture
  dragChart "13,184,98,268",70 -- Pile One
  dragChart "100,184,185,268",133 -- Pile Two
  dragChart "185,184,270,268",93 -- Pile Three
  dragChart "270,184,355,268",140 -- Pile Four
  dragChart "355,184,440,268",175 -- Pile Five
  choose browse tool
  wait 50
  hide card picture
  hide bkgnd field "Demo Field"
  set cantModify of this stack to false
end mouseUp

on dragChart theRect, theHeight
  put item 1 of theRect into theLeft
  put item 2 of theRect into theTop
  put item 3 of theRect into theRight
  put item 4 of theRect into theBottom
  choose select tool
  set the dragSpeed to 0
  <b>drag</b> from theLeft,theTop to theRight,theBottom with optionKey
  put round((theRight - theLeft)/2 + theLeft) into locH
  put round((theBottom - theTop)/2 + theTop) into locV
  doMenu "opaque"
  set the dragSpeed to 200
  <b>drag</b> from locH,locV to locH,(locV - theHeight) ¬
  with optionKey,commandKey
end dragChart
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [dragSpeed](/HyperTalkReference/properties/dragSpeed)
* [mouseLoc](/HyperTalkReference/functions/mouseLoc)
