---
title: do
card_id: 25485
modified: yes
---

# do

<code>do <i>expression</i> [as <i>scriptLanguage</i>]</code><br>
<br>
The<code> do </code>keyword forces HyperCard to evaluate<code> <i>expression</i> </code>and to send the result as a message to the current card.<br>
<br>
The value of<code> <i>expression</i> </code> can contain more than one line. For example, if you have a series of statements in a card field called Example, HyperCard will apply<code> do </code>to each line:<br>
<br>
<code>do card field "Example"</code><br>
<br>
When you use the <code>as <i>scriptLanguage </i></code>form, HyperCard executes the script in<code> <i>expression</i> </code>using the OSA-compliant scripting component named in <i><code>scriptLanguage</i>:<i><br>
<br>
</i>do field 1 as AppleScript do theScript as UserTalk</code><br>
<br>
You can also send<code> do </code>from the Message box.<br>

## Demo Script

<code><pre>
on doLast3Lines
  put the number of lines of bkgnd field "Demo Script" into N
  <b>do</b> line (N - 2) to N of bkgnd field "Demo Script"
end doLast3Lines

put sqrt(2)
beep
flash
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

## Related Topics

* [value](/HyperTalkReference/functions/value)
