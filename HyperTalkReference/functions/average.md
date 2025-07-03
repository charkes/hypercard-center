---
title: average
card_id: 52417
---

# average

`average([ph:numberList])`

Value returned:  number equal to the arithmetic average of the comma-separated list of numbers

## Examples

```
average(1,2,3,4,5,6,7,8,9,10)

repeat with N = 1 the number of lines of field "Number Data"
  put line N of field "Number Data" into item N of theNumbers
end repeat
put average(theNumbers)
```

## Demo Script

```
on onAverage
 repeat with numLine = 1 to the number of lines of me
   put the number of words of line numLine of me into¬
   item numLine of wordsInEachLine
 end repeat
 put "There are an average of" && <b>average</b>(wordsInEachLine) && ¬
 "words in each line of this field." into sayIt
 answer sayIt
end onAverage
```

## Related Topics

* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [max](/HyperTalkReference/functions/max)
* [min](/HyperTalkReference/functions/min)
