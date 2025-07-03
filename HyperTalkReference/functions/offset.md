---
title: offset
card_id: 60426
---

# offset

```
offset([ph:text1], [ph:text2])
```

Value returned: the number 0 if `[ph:text1]` does not appear in `[ph:text2]`; otherwise, a positive integer equal to the number of characters from the first character of `[ph:text2]` to the first character of `[ph:text1]` within `[ph:text2]` 

## Examples

```
get offset("world", "Hello world")

put offset(searchString,card field "Index") into theOffset

put offset(line 1 of card field 1, collectedHits) into N
if N is 0 then ...
else ...
```

## Demo Script

```
on answerDiskName
 answer "This stack resides on the disk named" && diskName() & "."
end answerDiskName
function diskName thelongName
 if thelongName is empty
 then put the long name of this stack into theLongName
 -- remove “stack "” from the beginning of theLongName
 delete char 1 to <b>offset</b>(quote,theLongName) of theLongName
 -- return word before the first “:”
 return char 1 to <b>offset</b>(":",theLongName) - 1 of theLongName
end diskName
```

## Related Topics

* [charToNum](/HyperTalkReference/functions/charToNum)
* [length](/HyperTalkReference/functions/length)
* [numToChar](/HyperTalkReference/functions/numToChar)
* [String operators](/HyperTalkReference/operatorsandconstants/String-operators)
