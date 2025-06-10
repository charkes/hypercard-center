---
title: repeat
card_id: 27427
modified: yes
---

# repeat

<code><pre>
repeat [forever]
   <i>statements</i>
end repeat
</pre></code>

<br>
The<code> </code>statements in a <code>repeat forever </code>structure repeat continuously.<br>
<br>
If HyperCard executes an<code> exit repeat </code>statement in the<code> </code>loop, it continues running the handler starting from the first statement after<code> end repeat</code>.<br>
<br>
If HyperCard executes a <code> next repeat </code>statement, it returns immediately to the beginning of the<code> repeat </code>loop.<br>

## Demo Script

<code><pre>
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
</pre></code>

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
