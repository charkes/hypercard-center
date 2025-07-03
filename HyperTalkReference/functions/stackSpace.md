---
title: stackSpace
card_id: 11662
---

# stackSpace

```
the stackSpace
stackSpace()
put the stackSpace into howMuch
```

Value returned: an integer representing the free space, in bytes, in HyperCard’s memory stack

The memory that HyperCard can use is divided into two parts—the heap and the stack. `HeapSpace` returns the amount of memory that’s available in the heap portion. `StackSpace` returns the amount that’s available in the stack portion.

The memory in HyperCard’s stack determines, for example, the number of times you can call a recursive handler.

## Examples

```
put stackSpace() into roomEnough
if roomEnough > 8000 then ...
```

## Related Topics

* [heapSpace](/HyperTalkReference/functions/heapSpace)
