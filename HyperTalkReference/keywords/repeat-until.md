---
title: repeat until
card_id: 28073
modified: yes
---

# repeat until

<code><pre>
repeat until <i>trueOrFalse</i>
   <i>statements</i>
end repeat
</pre></code>

<br>
The statements in a<code> repeat until </code>structure repeat as long as the condition following the word<code> until </code>is false. HyperCard checks the condition before the first and any subsequent iterations of the loop.<br>
<br>
If HyperCard executes an<code> exit repeat </code>statement in the<code> </code>loop, it continues running the handler starting from the first statement after<code> end repeat</code>.<br>
<br>
If HyperCard executes a <code>next repeat </code>statement, it returns immediately to the beginning of the<code> repeat </code>loop.<br>

## Demo Script

<code><pre>
on mouseUp
  show bkgnd field "demo field"
  put return & "    Point at the number to stop counting..." ¬
  into bkgnd field "demo field"
  put 0 into theCount
  put space & space & theCount after bkgnd field "demo field"
  <b>repeat until</b> the mouseLoc is within "321,81,370,110"
    add 1 to theCount
    put theCount into last word of bkgnd field "demo field"
    if theCount = 100 then exit repeat -- just in case.
  <b>end repeat</b>
  wait 20
  hide bkgnd field "demo field"
  put empty into bkgnd field "demo field"
end mouseUp
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/trueOrFalse.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
