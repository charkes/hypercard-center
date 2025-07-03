---
title: numToChar
card_id: 60292
---

# numToChar

```
the numToChar of [ph:posInteger]
```

Value returned: the character whose ASCII equivalent equals `[ph:posInteger]`

## Examples

```
the numToChar of 65
numToChar(65)

put charToNum(numToChar(65)) = 65
```

## Demo Script

```
on nameUpperCase
 ask "Please enter your name:"
 if it is empty then exit nameUpperCase
 answer uppercase(it)
end nameUpperCase
function upperCase whatStr
 repeat with charNum = 1 to the number of chars in whatStr
   put charToNum(char charNum of whatStr) into thisChar
   if thisChar ≥ 97 AND thisChar ≤ 122
   then put <b>numToChar</b>(thisChar - 32) into char charNum of whatStr
 end repeat
 return whatStr
end upperCase
```

## Related Topics

* [charToNum](/HyperTalkReference/functions/charToNum)
* [length](/HyperTalkReference/functions/length)
* [offset](/HyperTalkReference/functions/offset)
* [String operators](/HyperTalkReference/operatorsandconstants/String-operators)
