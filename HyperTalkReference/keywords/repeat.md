---
title: repeat
card_id: 27427
modified: yes
---

# repeat

```
repeat [forever]
   [ph:statements]
end repeat
```

The statements in a `repeat forever` structure repeat continuously.

If HyperCard executes an `exit repeat` statement in the loop, it continues running the handler starting from the first statement after `end repeat`.

If HyperCard executes a `next repeat` statement, it returns immediately to the beginning of the `repeat` loop.

## Demo Script

```
on mouseUp
  show bkgnd field "demo field"
  put return & "    Click the mouse to stop counting..." ¬
  into bkgnd field "demo field"
  put 1 into theCount
  put space & space & theCount after bkgnd field "demo field"
  <b>repeat</b> <b>forever
</b>    set the cursor to busy
    add 1 to theCount
    get last char of theCount
    if it = 0 OR it = 5 then <b>next repeat</b> -- skip fives and tens
    put theCount into last word of bkgnd field "demo field"
    if the mouse is DOWN OR theCount = 10000 then <b>exit repeat</b>
 <b> end repeat</b>
  hide bkgnd field "demo field"
  put empty into bkgnd field "demo field"
end mouseUp
```

## Placeholders

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
