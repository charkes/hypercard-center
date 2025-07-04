---
title: size
card_id: 83131
---

# size

` the size of [ph:stack`]

The `size` property returns the size of the specified stack in bytes.

The `size` property can’t be changed with the `set` command. It’s changed only by adding and deleting objects and graphics from a stack. You must compact the stack to recover the space occupied by the deleted objects and graphics. 


## Examples

```
the size of this stack
the size of stack "home"
```

## Demo Script

```
on stackSize
  answer "The size of this stack is" &&¬
  (the <b>size</b> of this stack) div 1024 & "K bytes."
end stackSize
```

## Related Topics

* [diskSpace](/HyperTalkReference/functions/diskSpace)
* [freeSize](/HyperTalkReference/properties/freeSize)
