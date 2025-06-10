---
title: function
card_id: 25888
modified: yes
---

# function

<code><pre>
function <i>functionName</i> [<i>parameterList</i>]
  <i>statements</i>
end <i>functionName</i>
</pre></code>

<br>
The<code> function </code>keyword defines a new function handler of the specified name.  You call a function by placing parentheses after its name, enclosing any parameters within the parentheses:<br>
<br>
<code>get deleteSpaces(" hello ")</code><br>
<br>
The optional<code> <i>parameterList</i> </code>lets a function handler receive values sent along with the function call.<br>
<br>
When a function is called, HyperCard evaluates each item within the parenthetical list following the function's name.  When the handler begins to execute, HyperCard assigns each value to a parameter variable  in the<code> <i>parameterList</i></code>.<br>
<br>
Use the<code> return </code>keyword within the function definition to have the function return a value to the handler that called it. If you don't use<code> return</code>, the function evaluates to<code> empty</code>.<br>

## Demo Script

<code><pre>
on mouseUp
  ask "What is your name?"
  if it is empty then exit mouseUp
  answer "Your name spelled backwards is" && reverseString(it) & "."
end mouseUp

<b>function</b> reverseString theString
  repeat with i = the number of chars in theString down to 1
    put char i of theString after theReversedString
  end repeat
  return theReversedString
end reverseString
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/functionName.md]

[embed:HelpExtras/Placeholders/parameterList.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [exit](/HyperTalkReference/keywords/exit)
* [param](/HyperTalkReference/functions/param)
* [paramCount](/HyperTalkReference/functions/paramCount)
* [params](/HyperTalkReference/functions/params)
* [return](/HyperTalkReference/keywords/return)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
* [Using parameter variables](/HyperTalkReference/hypertalkbasics/Using-parameter-variables)
* [Writing function handlers](/HyperTalkReference/hypertalkbasics/Writing-function-handlers)
