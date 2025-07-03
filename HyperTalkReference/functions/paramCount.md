---
title: paramCount
card_id: 61390
---

# paramCount

```
the paramCount
```

Value returned: a positive integer equal to the total number of parameters passed to the current handler

## Demo Script

```
on paramDemo
  showParams 1, "a", "this is fun", the number of cards
end paramDemo
on showParams
  repeat with N = 0 to <b>the paramCount</b>
    put N & ":" && space && param(N) & return after theMessage
  end repeat
  answer "The parameters are:" & return & return & theMessage
end showParams
```

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [param](/HyperTalkReference/functions/param)
* [params](/HyperTalkReference/functions/params)
