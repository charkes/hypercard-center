---
title: mouse
card_id: 58372
---

# mouse

<code><pre>
the mouse
</pre></code>

Value returned: one of the constants <code>up</code> or <code>down</code> indicating whether the mouse button is up or down<code>

</code>Note: Use <code>the mouse</code> to return  the current state of the mouse  button and <code>the mouseClick </code>to  return whether the mouse has been clicked in the current handler. 


## Examples

```
if the mouse is up then ...

if (the mouse is down) or (the commandKey is down) then ...

wait until the mouse is up
```

## Demo Script

<code><pre>
on theMouse
  show bkgnd field "demo field"
  displayMessage "Click the mouse to continue . . ."
  wait until the<b> mouse</b> is down
  hide bkgnd field "demo field"
end theMouse
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouseClick](/HyperTalkReference/functions/mouseClick)
