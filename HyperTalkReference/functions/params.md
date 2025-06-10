---
title: params
card_id: 61645
---

# params

<code><pre>
the params
</pre></code>

Value returned: a text string equal to the entire parameter list, including the message name, passed to the currently executing handler 


## Demo Script

<code><pre>
<code><pre>
on paramsDemo
  showParams 1, "a", "this is fun", the number of cards
end paramsDemo
on showParams
   answer "The parameters are:" & return & return & the params
end showParams
</pre></code>
</pre></code>

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [param](/HyperTalkReference/functions/param)
* [paramCount](/HyperTalkReference/functions/paramCount)
