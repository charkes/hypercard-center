---
title: repeat for
card_id: 27895
modified: yes
---

# repeat for

<code><pre>
repeat [for] <i>posInteger</i> [times]
   <i>statements</i>
end repeat
</pre></code>

<br>
The statements in a<code> repeat for </code>structure repeat for a specified number of times.<br>
<br>
If HyperCard executes an<code> exit repeat </code>statement in the<code> </code>loop, it continues running the handler starting from the first statement after<code> end repeat</code>.<br>
<br>
If HyperCard executes a <code>next repeat </code>statement, it returns immediately to the beginning of the<code> repeat </code>loop.<br>

## Demo Script

<code><pre>
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
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/posInteger.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [exit](/HyperTalkReference/keywords/exit)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
