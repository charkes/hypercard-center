---
title: function
card_id: 25888
modified: yes
---

# function

```
function [ph:functionName] [[ph:parameterList]]
  [ph:statements]
end [ph:functionName]
```

The `function` keyword defines a new function handler of the specified name.  You call a function by placing parentheses after its name, enclosing any parameters within the parentheses:

`get deleteSpaces(" hello ")`

The optional `[ph:parameterList]` lets a function handler receive values sent along with the function call.

When a function is called, HyperCard evaluates each item within the parenthetical list following the function's name.  When the handler begins to execute, HyperCard assigns each value to a parameter variable  in the<code> [ph:parameterList]</code>.

Use the `return` keyword within the function definition to have the function return a value to the handler that called it. If you don't use<code> return</code>, the function evaluates to `empty`.

## Demo Script

```
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
```

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
