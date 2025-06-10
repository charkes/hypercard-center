---
title: optionKey
card_id: 60915
---

# optionKey

<code><pre>
the optionKey
</pre></code>

Value returned: one of the constants <code>up</code> or <code>down</code> indicating whether the Option key is up or down 


## Examples

```
if the optionKey is up then ...

if (the mouse is down) and (the optionKey is down) then...

wait until optionKey() is up
```

## Demo Script

<code><pre>
on optionKeyDemo
  -- Hold down the Option key when you click Run the Script.
  answer "The Option key is:" && the <b>optionKey</b>
end optionKeyDemo
</pre></code>

## Related Topics

* [commandKey](/HyperTalkReference/functions/commandKey)
* [shiftKey](/HyperTalkReference/functions/shiftKey)
