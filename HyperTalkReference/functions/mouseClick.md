---
title: mouseClick
card_id: 58695
---

# mouseClick

<code><pre>
the mouseClick
</pre></code>

Value returned: the constant<code> true </code>if the mouse has been clicked sometime during the running of the current handler, or <code>false</code> if it hasn't.

If the mouse button is down,<code> the mouseClick </code>waits until the mouse button is up before returning<code> true</code>. 



Note: Use <code>the mouse</code> to return  the current state of the mouse  button and <code>the mouseClick </code>to  return whether the mouse has been clicked in the current handler. 


## Examples

```
if the mouseClick then ...

if (the mouseClick) or (the commandKey is down) then ...

repeat until the mouseClick
 ...
end repeat
```

## Demo Script

<code><pre>
<code><pre>
on theMouseClick
 show bkgnd field "demo field"
 displayMessage "Click the mouse to continue . . ."
 wait until the <b>mouseClick</b>
 hide bkgnd field "demo field"
end theMouseClick
</pre></code>
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouse](/HyperTalkReference/functions/mouse)
