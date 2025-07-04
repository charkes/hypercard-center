---
title: if (multiple-statement)
card_id: 26404
modified: yes
---

# if (multiple-statement)

```
if [ph:trueOrFalse] then
    [ph:statements]
[else if [ph:trueOrFalse] then
   [ph:statements]]
[else
    [ph:statements]]
end if
```

The multiple-statement `if` structure tests the specified condition and executes <b>one or more</b> statements if the condition is true. You use the optional `else if` or `else` form to run alternative blocks of code in case the  condition following `if` is false.

Because each part of a complex `if` structure may contain more than one statement, you must have an `end if` statement at the end of the structure.

## Demo Script

```
on mouseUp
 put random(19) into theNumber
 put 0 into botNum
 put 20 into topNum
 put 0 into numberOfTrys
 put "I am thinking of a number between 0 and 20." & return & ¬
 "Try to guess the number:" into sayIt
 repeat
   add 1 to numberOfTrys
   ask sayIt
   <b>if</b> the result is "Cancel" OR it is empty then exit repeat
   put it into theGuess
   <b>if</b> theGuess = theNumber then
     answer "You got it! The number is" && theGuess & "." & return &¬
     "You guessed in" && numberOfTrys && "attempts."
     exit repeat
   <b>else if</b> theGuess is not a number then
    put theGuess && "is not a number." into sayIt
   <b>else</b> <b>if</b> theGuess > topNum then
     put theGuess && "is greater than" && topNum & "." into sayIt
   <b>else</b> <b>if</b> theGuess < botNum then
     put theGuess && "is less than" && botNum & "." into sayIt
   <b>else</b> <b>if</b> theGuess < theNumber then
     put "The number is greater than" && theGuess & "." into sayIt
     put theGuess into botNum
   <b>else</b> <b>if</b> theGuess > theNumber then
     put "The number is less than" && theGuess & "." into sayIt
     put theGuess into topNum
   <b>end</b> <b>if
</b>    put return & "Please enter a number between" && botNum &&¬
   "and" && topNum & ":" after sayIt
 end repeat
end mouseUp
```

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
