---
title: mouseClick
card_id: 58695
---

# mouseClick

```
the mouseClick
```

Value returned: the constant `true` if the mouse has been clicked sometime during the running of the current handler, or `false` if it hasn't.

If the mouse button is down, `the mouseClick` waits until the mouse button is up before returning `true`.

Note: Use `the mouse` to return the current state of the mouse button and `the mouseClick` to return whether the mouse has been clicked in the current handler. 

## Examples

```
if the mouseClick then ...

if (the mouseClick) or (the commandKey is down) then ...

repeat until the mouseClick
 ...
end repeat
```

## Demo Script

```
on theMouseClick
 show bkgnd field "demo field"
 displayMessage "Click the mouse to continue . . ."
 wait until the <b>mouseClick</b>
 hide bkgnd field "demo field"
end theMouseClick
```

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouse](/HyperTalkReference/functions/mouse)
