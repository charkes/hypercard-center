---
title: shiftKey
card_id: 64480
---

# shiftKey

<code><pre>
the shiftKey
</pre></code>

Value returned: one of the constants<code> up </code>or <code>down</code> indicating whether the Shift key is up or down 


## Examples

```
if the shiftKey is up then ...

if (the mouse is down) and (the shiftKey is down) then...

wait until shiftKey() is up
```

## Demo Script

<code><pre>
on shiftKeyDemo
  -- Hold down the Shift key when you click Run the Script.
  answer "The Shift key is:" && the <b>shiftKey</b>
end shiftKeyDemo
</pre></code>

## Related Topics

* [commandKey](/HyperTalkReference/functions/commandKey)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [optionKey](/HyperTalkReference/functions/optionKey)
