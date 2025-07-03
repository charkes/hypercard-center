---
title: shiftKey
card_id: 64480
---

# shiftKey

```
the shiftKey
```

Value returned: one of the constants `up` or `down` indicating whether the Shift key is up or down 

## Examples

```
if the shiftKey is up then ...

if (the mouse is down) and (the shiftKey is down) then...

wait until shiftKey() is up
```

## Demo Script

```
on shiftKeyDemo
  -- Hold down the Shift key when you click Run the Script.
  answer "The Shift key is:" && the <b>shiftKey</b>
end shiftKeyDemo
```

## Related Topics

* [commandKey](/HyperTalkReference/functions/commandKey)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [optionKey](/HyperTalkReference/functions/optionKey)
