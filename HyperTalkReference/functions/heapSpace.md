---
title: heapSpace
card_id: 56991
---

# heapSpace

<code><pre>
the heapSpace
</pre></code>

Value returned: a number equal to the amount of working memory HyperCard has left (the number of bytes remaining in HyperCard’s application heap)

The memory that HyperCard can use is divided into two parts—the heap and the stack. <code>StackSpace</code>  returns the amount of memory that’s available in the stack portion. <code>HeapSpace</code> returns the amount available in the heap portion.  


The available memory determines whether the user can use the Paint tools, whether HyperCard can open a stack in a new window, and other performance-related factors.

## Examples

```
get the heapSpace()
if it < 100 then ...
```

## Related Topics

* [stackSpace](/HyperTalkReference/functions/stackSpace)
