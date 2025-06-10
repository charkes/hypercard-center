---
title: click at
card_id: 32047
---

# click at

<code>click at [ph:point] </code>
<code>click at [ph:point] with [ph:key1</code>] <code>click at [ph:point] with [ph:key1], [ph:key2</code>] <code>click at [ph:point] with [ph:key1], [ph:key2], [ph:key3</code>] 

The <code>click at</code> command clicks the mouse from within scripts. It acts exactly as if the user had clicked the mouse on the screen. 

If <code>[ph:point]</code> is within the rectangle of a button, a locked field, or anywhere else on the card, HyperCard sends the <code>mouseDown</code>, <code>mouseStillDown</code>, and <code>mouseUp</code> messages to the object. 

If <code>[ph:point]</code> is within the rectangle of an unlocked field, HyperCard sets the insertion point in the field.

The <code>with [ph:key]</code> options specify combinations of the <code>commandKey</code>, the <code>optionKey</code>, and the <code>shiftKey</code>, just as if the user were holding down the key or keys while clicking the mouse. 


## Examples

```
click at 0,0

click at the mouseLoc

click at the mouseLoc with shiftKey,optionKey -- Option-Shift-click
```

## Demo Script

<code><pre>
on clickAtCloseBox
  -- Close this demo field.
  <b>click</b> at the loc of bkgnd button "close"
end clickAtCloseBox
</pre></code>

## Related Topics

* [clickH and clickV](/HyperTalkReference/functions/clickH-and-clickV)
* [clickLoc](/HyperTalkReference/functions/clickLoc)
* [drag](/HyperTalkReference/commands/drag)
* [mouse](/HyperTalkReference/functions/mouse)
* [mouseClick](/HyperTalkReference/functions/mouseClick)
* [mouseLoc](/HyperTalkReference/functions/mouseLoc)
* [select](/HyperTalkReference/commands/select)
* [selectedLoc](/HyperTalkReference/functions/selectedLoc)
* [type](/HyperTalkReference/commands/type)
