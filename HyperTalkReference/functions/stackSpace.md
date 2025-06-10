---
title: stackSpace
card_id: 11662
---

# stackSpace

<code><pre>
the stackSpace
stackSpace()
put the stackSpace into howMuch
</pre></code>

Value returned: an integer representing the free space, in bytes, in HyperCard’s memory stack

The memory that HyperCard can use is divided into two parts—the heap and the stack. <code>HeapSpace</code>  returns the amount of memory that’s available in the heap portion. <code>StackSpace</code> returns the amount that’s available in the stack portion. 



The memory in HyperCard’s stack determines, for example, the number of times you can call a recursive handler.

## Examples

```
put stackSpace() into roomEnough
if roomEnough > 8000 then ...
```

## Related Topics

* [heapSpace](/HyperTalkReference/functions/heapSpace)
