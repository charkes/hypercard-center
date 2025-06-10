---
title: repeat with
card_id: 28477
modified: yes
---

# repeat with

<code><pre>
repeat with <i>variableName</i> = ¬
    <i>integer1</i> to <i>integer2</i>
    <i>statements</i>
end repeat

repeat with <i>variableName</i> = ¬
    <i>integer1</i> down to <i>integer2</i>
    <i>statements</i>
end repeat
</pre></code>

<br>
The statements in a<code> repeat with </code>structure repeat until a variable with an initial value of<code> <i>integer1</i> </code>is greater than (or, in the case of <code>down to</code>, less than) the number <i><code>integer2</i></code>.<br>
<br>
The value of the variable increases (or decreases) by 1 during each iteration of the<code> repeat </code>loop.<br>
<br>
If HyperCard executes an<code> exit repeat </code>statement in the<code> </code>loop, it continues running the handler starting from the first statement after<code> end repeat</code>. If HyperCard executes a<code> next repeat </code>statement, it returns immediately to the beginning of the<code> repeat </code>loop  and increases (or decreases) the value of the variable.<br>

## Demo Script

<code><pre>
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
</pre></code>

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
