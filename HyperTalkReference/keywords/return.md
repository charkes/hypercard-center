---
title: return
card_id: 28715
modified: yes
---

# return

`return [ph:expression]`

The `return` keyword ends execution of a handler and, in function handlers, returns the value of `[ph:expression]` to the handler that called the function.

If `return` appears in a message handler (as opposed to a function handler), it ends execution of the handler and places the value of the expression into the HyperTalk function `the result`.

The value of `the result` as set by a `return` statement is valid only immediately after the `return` statement executes; each new statement resets `the result` to `empty`.

## Demo Script

```
on whatDisk
 answer "This stack resides on the disk named" && diskName() & "."
end whatDisk
function diskName longStackName
 if longStackName is empty
 then put the long name of this stack into longStackName
 delete char 1 to 7 of longStackName -- remove “stack "”
 <b>return</b> char 1 to (offset(":",longStackName) - 1) of longStackName
end diskName
```

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [result](/HyperTalkReference/functions/result)
