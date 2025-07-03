---
title: optionKey
card_id: 60915
---

# optionKey

```
the optionKey
```

Value returned: one of the constants `up` or `down` indicating whether the Option key is up or down


## Examples

```
if the optionKey is up then ...

if (the mouse is down) and (the optionKey is down) then...

wait until optionKey() is up
```

## Demo Script

```
on optionKeyDemo
  -- Hold down the Option key when you click Run the Script.
  answer "The Option key is:" && the <b>optionKey</b>
end optionKeyDemo
```

## Related Topics

* [commandKey](/HyperTalkReference/functions/commandKey)
* [shiftKey](/HyperTalkReference/functions/shiftKey)
