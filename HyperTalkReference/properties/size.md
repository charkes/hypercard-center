---
title: size
card_id: 83131
---

# size

<code> the size of [ph:stack</code>]

The <code>size</code> property returns the size of the specified stack in bytes.

The <code>size</code> property can’t be changed with the <code>set</code> command. It’s changed only by adding and deleting objects and graphics from a stack. You must compact the stack to recover the space occupied by the deleted objects and graphics. 


## Examples

```
the size of this stack
the size of stack "home"
```

## Demo Script

<code><pre>
on stackSize
  answer "The size of this stack is" &&¬
  (the <b>size</b> of this stack) div 1024 & "K bytes."
end stackSize
</pre></code>

## Related Topics

* [diskSpace](/HyperTalkReference/functions/diskSpace)
* [freeSize](/HyperTalkReference/properties/freeSize)
