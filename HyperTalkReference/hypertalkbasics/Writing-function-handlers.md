---
title: Writing function handlers
card_id: 10397
modified: yes
---

# Writing function handlers

When you write a handler for a function, you specify statements that compute and return a value to the handler that calls the function. Each function handler has the following form, where the italicized words are placeholders:

<code><pre>
function <i>functionName</i>
    <i>statements</i>
end <i>functionName</i>
</pre></code>

HyperCard has many built-in functions, but you can also write your own:

<code><pre>
on mouseUp
   put square(5) into the Message box
end mouseUp

function square x
   return (x * x)
end square
</pre></code>


The function <code>square</code> receives a number through its parameter variable, <code>x</code>.  It then returns the value of <code> x * x</code> to the handler that called it (<code>mouseUp</code>) using the <code>return</code> keyword.

## Placeholders

[embed:HelpExtras/Placeholders/functionName.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [The building blocks](/HyperTalkReference/hypertalkbasics/The-building-blocks)
* [Using parameter variables](/HyperTalkReference/hypertalkbasics/Using-parameter-variables)
