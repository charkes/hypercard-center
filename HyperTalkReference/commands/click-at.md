---
title: click at
card_id: 32047
---

# click at

`click at [ph:point]`
`click at [ph:point] with [ph:key1]`
`click at [ph:point] with [ph:key1], [ph:key2]`
`click at [ph:point] with [ph:key1], [ph:key2], [ph:key3]`

The `click at` command clicks the mouse from within scripts. It acts exactly as if the user had clicked the mouse on the screen.

If `[ph:point]` is within the rectangle of a button, a locked field, or anywhere else on the card, HyperCard sends the `mouseDown`, `mouseStillDown`, and `mouseUp` messages to the object.

If `[ph:point]` is within the rectangle of an unlocked field, HyperCard sets the insertion point in the field.

The `with [ph:key]` options specify combinations of the `commandKey`, the `optionKey`, and the `shiftKey`, just as if the user were holding down the key or keys while clicking the mouse.

## Examples

```
click at 0,0

click at the mouseLoc

click at the mouseLoc with shiftKey,optionKey -- Option-Shift-click
```

## Demo Script

```
on clickAtCloseBox
  -- Close this demo field.
  <b>click</b> at the loc of bkgnd button "close"
end clickAtCloseBox
```

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
