---
title: repeat with
card_id: 28477
modified: yes
---

# repeat with

```
repeat with [ph:variableName] = ¬
    [ph:integer1] to [ph:integer2]
    [ph:statements]
end repeat

repeat with [ph:variableName] = ¬
    [ph:integer1] down to [ph:integer2]
    [ph:statements]
end repeat
```

The statements in a `repeat with` structure repeat until a variable with an initial value of `[ph:integer1]` is greater than (or, in the case of <code>down to</code>, less than) the number `[ph:integer2]`.

The value of the variable increases (or decreases) by 1 during each iteration of the `repeat` loop.

If HyperCard executes an `exit repeat` statement in the loop, it continues running the handler starting from the first statement after `end repeat`. If HyperCard executes a `next repeat` statement, it returns immediately to the beginning of the `repeat` loop  and increases (or decreases) the value of the variable.

## Demo Script

```
on mouseUp
  show bkgnd field "demo field"
  put return & spaces(25) & "Counting down to 0:  10" ¬
  into bkgnd field "demo field"
  <b>repeat with</b> theCount = 10 down to 0
    put theCount into last word of bkgnd field "demo field"
    wait 15 ticks
  <b>end repeat</b>
  flash
  wait 20
  hide bkgnd field "demo field"
  put empty into bkgnd field "demo field"
end mouseUp
```

## Placeholders

[embed:HelpExtras/Placeholders/variableName.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
