---
title: return
card_id: 28715
modified: yes
---

# return

<code>return <i>expression</i></code><br>
<br>
The<code> return </code>keyword ends execution of a handler and, in function handlers, returns the value of<code> <i>expression</i> </code>to the handler that called the function.<br>
<br>
If<code> return </code>appears in a message handler (as opposed to a function handler), it ends execution of the handler and places the value of the expression into the HyperTalk function<code> the result</code>.<br>
<br>
The value of<code> the result </code>as set by a<code> return </code>statement is valid only immediately after the<code> return </code>statement executes; each new statement resets<code> the result </code>to<code> empty.</code><br>

## Demo Script

<code><pre>
<code><pre>
on whatDisk
 answer "This stack resides on the disk named" && diskName() & "."
end whatDisk
function diskName longStackName
 if longStackName is empty
 then put the long name of this stack into longStackName
 delete char 1 to 7 of longStackName -- remove “stack "”
 <b>return</b> char 1 to (offset(":",longStackName) - 1) of longStackName
end diskName
</pre></code>
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [result](/HyperTalkReference/functions/result)
