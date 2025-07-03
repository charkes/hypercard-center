---
title: length
card_id: 57200
---

# length

```
the length of [ph:expression]
```

Value returned: the number of characters in the value of the expression 

## Examples

```
length of "Hello world"
length("Hello world")

length of field "Index"
length of myVar

length of 3 + 2 -- returns 3
length of (3+2) -- returns 1
```

## Demo Script

```
on lengthOfMe
 put the <b>length</b> of bkgnd field "Demo Script" into numChars
 answer "This demo script contains" && numChars && "characters."
end lengthOfMe
```

## Related Topics

* [charToNum](/HyperTalkReference/functions/charToNum)
* [numToChar](/HyperTalkReference/functions/numToChar)
* [offset](/HyperTalkReference/functions/offset)
* [String operators](/HyperTalkReference/operatorsandconstants/String-operators)
