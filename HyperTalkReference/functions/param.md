---
title: param
card_id: 61134
---

# param

```
the param of [ph:posInteger]
```

Value returned: the value (as opposed to the name) of a parameter variable in the current handler, or `empty` if the parameter variable doesn't exist

The `param of 0` is the name of the message itself.

## Examples

```
param of 1
param(1)

put param(0) into theMessageName
```

## Demo Script

```
on paramDemo
  showParams 1, "a", "this is fun", the number of cards
end paramDemo
on showParams
  repeat with N = 0 to the paramCount
    put N & ":" && space && <b>param</b>(N) & return after theMessage
  end repeat
  answer "The parameters are:" & return & return & theMessage
end showParams
```

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [paramCount](/HyperTalkReference/functions/paramCount)
* [params](/HyperTalkReference/functions/params)
