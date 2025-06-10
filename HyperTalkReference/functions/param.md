---
title: param
card_id: 61134
---

# param

<code><pre>
the param of [ph:posInteger]
</pre></code>

Value returned: the value (as opposed to the name) of a parameter variable in the current handler, or <code>empty</code> if the parameter variable doesn't exist

The <code>param of 0</code> is the name of the message itself. 


## Examples

```
param of 1
param(1)

put param(0) into theMessageName
```

## Demo Script

<code><pre>
<code><pre>
on paramDemo
  showParams 1, "a", "this is fun", the number of cards
end paramDemo
on showParams
  repeat with N = 0 to the paramCount
    put N & ":" && space && <b>param</b>(N) & return after theMessage
  end repeat
  answer "The parameters are:" & return & return & theMessage
end showParams
</pre></code>
</pre></code>

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [paramCount](/HyperTalkReference/functions/paramCount)
* [params](/HyperTalkReference/functions/params)
