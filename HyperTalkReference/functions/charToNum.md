---
title: charToNum
card_id: 52559
---

# charToNum

<code><pre>
the charToNum of [ph:char]
</pre></code>

Value returned: positive integer equal to the ASCII value of the<code> [ph:char</code>] 


## Examples

```
the charToNum of "A"
charToNum("A")

put numToChar(charToNum("A")) = "A"
```

## Demo Script

<code><pre>
on nameUpperCase
  ask "Please enter your name:"
  if (it is empty) or (the result is "Cancel") then exit nameUpperCase
  answer uppercase(it)
end nameUpperCase

function upperCase whatStr
  repeat with charNum = 1 to the number of chars in whatStr
    put <b>charToNum</b>(char charNum of whatStr) into thisChar
    if thisChar ≥ 97 AND thisChar ≤ 122
    then put numToChar(thisChar - 32) into char charNum of whatStr
  end repeat
  return whatStr
end upperCase
</pre></code>

## Related Topics

* [length](/HyperTalkReference/functions/length)
* [numToChar](/HyperTalkReference/functions/numToChar)
* [offset](/HyperTalkReference/functions/offset)
* [String operators](/HyperTalkReference/operatorsandconstants/String-operators)
