---
title: repeat for
card_id: 27895
modified: yes
---

# repeat for

```
repeat [for] [ph:posInteger] [times]
   [ph:statements]
end repeat
```

The statements in a `repeat for` structure repeat for a specified number of times.

If HyperCard executes an `exit repeat` statement in the loop, it continues running the handler starting from the first statement after `end repeat`.

If HyperCard executes a `next repeat` statement, it returns immediately to the beginning of the `repeat` loop.

## Demo Script

```
on mouseUp
  show bkgnd field "demo field"
  put return & "    The count will stop at 10:" ¬
  into bkgnd field "demo field"
  put 0 into theCount
  put space & space & theCount after bkgnd field "demo field"
  <b>repeat for</b> 10 times
    add 1 to theCount
    put theCount into last word of bkgnd field "demo field"
  <b>end repeat</b>
  wait 30
  hide bkgnd field "demo field"
  put empty into bkgnd field "demo field"
end mouseUp
```

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
