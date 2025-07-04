---
title: freeSize
card_id: 72105
---

# freeSize

`the freeSize of [ph:stack`]

The `freeSize` property returns the amount of free space, in bytes, in the specified stack. (Free space is created in a stack each time you add or delete an object or graphics.) 

To set the `freeSize` property to 0, choose Compact Stack from the File menu or use the command 

`doMenu "Compact Stack"`

from a handler or the Message box. 


## Examples

```
get the freeSize of this stack
if it > 10240 then doMenu "Compact Stack"
```

## Demo Script

```
on checkFreeSize
  get the <b>freeSize</b> of this stack
  answer "The freeSize of this stack is" && it div 1024 & "K."
end checkFreeSize
```

## Related Topics

* [diskSpace](/HyperTalkReference/functions/diskSpace)
* [size](/HyperTalkReference/properties/size)
