---
title: Writing function handlers
card_id: 10397
modified: yes
---

# Writing function handlers

When you write a handler for a function, you specify statements that compute and return a value to the handler that calls the function. Each function handler has the following form, where the italicized words are placeholders:

```
function [ph:functionName]
    [ph:statements]
end [ph:functionName]
```

HyperCard has many built-in functions, but you can also write your own:

```
on mouseUp
   put square(5) into the Message box
end mouseUp

function square x
   return (x * x)
end square
```

The function `square` receives a number through its parameter variable, `x`.  It then returns the value of `x * x` to the handler that called it (`mouseUp`) using the `return` keyword.

## Placeholders

[embed:HelpExtras/Placeholders/functionName.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [The building blocks](/HyperTalkReference/hypertalkbasics/The-building-blocks)
* [Using parameter variables](/HyperTalkReference/hypertalkbasics/Using-parameter-variables)
