---
title: freeSize
card_id: 72105
---

# freeSize

<code>the freeSize of [ph:stack</code>]

The <code>freeSize</code> property returns the amount of free space, in bytes, in the specified stack. (Free space is created in a stack each time you add or delete an object or graphics.) 

To set the <code>freeSize</code> property to 0, choose Compact Stack from the File menu or use the command 

<code>doMenu "Compact Stack"</code>

from a handler or the Message box. 


## Examples

```
get the freeSize of this stack
if it > 10240 then doMenu "Compact Stack"
```

## Demo Script

<code><pre>
on checkFreeSize
  get the <b>freeSize</b> of this stack
  answer "The freeSize of this stack is" && it div 1024 & "K."
end checkFreeSize
</pre></code>

## Related Topics

* [diskSpace](/HyperTalkReference/functions/diskSpace)
* [size](/HyperTalkReference/properties/size)
