---
title: repeat while
card_id: 28298
modified: yes
---

# repeat while

```
repeat while <i>trueOrFalse</i>
   <i>statements</i>
end repeat
```

The statements in a `repeat while` structure repeat as long as the condition following the word `while` is true. HyperCard checks the condition before the first and any subsequent iterations of the loop.

If HyperCard executes an `exit repeat` statement in the loop, it continues running the handler starting from the first statement after `end repeat`.

If HyperCard executes a `next repeat` statement, it returns immediately to the beginning of the `repeat` loop.

## Demo Script

```
on mouseUp
  show bkgnd field "demo field"
  put return & "    Press the mouse to stop counting..." ¬
  into bkgnd field "demo field"
  put 0 into theCount
  put space & space & theCount after bkgnd field "demo field"
 <b> repeat while</b> the mouse is up
    add 1 to theCount
    put theCount into last word of bkgnd field "demo field"
  <b>end repeat</b>
  wait 20
  hide bkgnd field "demo field"
  put empty into bkgnd field "demo field"
end mouseUp
```

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
