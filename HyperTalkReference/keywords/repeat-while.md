---
title: repeat while
card_id: 28298
modified: yes
---

# repeat while

<code><pre>
repeat while <i>trueOrFalse</i>
   <i>statements</i>
end repeat
</pre></code>

<br>
The statements in a <code>repeat while</code> structure repeat as long as the condition following the word<code> while </code>is true. HyperCard checks the condition before the first and any subsequent iterations of the loop.<br>
<br>
If HyperCard executes an<code> exit repeat </code>statement in the<code> </code>loop, it continues running the handler starting from the first statement after<code> end repeat</code>.<br>
<br>
If HyperCard executes a<code> next repeat </code>statement, it returns immediately to the beginning of the<code> repeat </code>loop.<br>

## Demo Script

<code><pre>
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
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
