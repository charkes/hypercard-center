---
title: mouse
card_id: 58372
---

# mouse

```
the mouse
```

Value returned: one of the constants `up` or `down` indicating whether the mouse button is up or down

Note: Use `the mouse` to return the current state of the mouse  button and `the mouseClick` to return whether the mouse has been clicked in the current handler. 

## Examples

```
if the mouse is up then ...

if (the mouse is down) or (the commandKey is down) then ...

wait until the mouse is up
```

## Demo Script

```
on theMouse
  show bkgnd field "demo field"
  displayMessage "Click the mouse to continue . . ."
  wait until the<b> mouse</b> is down
  hide bkgnd field "demo field"
end theMouse
```

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouseClick](/HyperTalkReference/functions/mouseClick)
