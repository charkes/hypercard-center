---
title: userModify
card_id: 87651
---

# userModify

<code> set </code>[<code>the</code>]<code> userModify to [ph:trueOrFalse] </code> The <code>userModify</code> property returns or sets whether the user can temporarily type into fields, use the Paint tools, and move or delete objects in a locked stack.

HyperCard discards any changes made by the user or a handler when it leaves the card, although a handler can record the changes and save them to another stack or file. 

 The <code>userModify</code> is set to false when the user changes stacks or quits HyperCard.

Note: <code>userModify</code> has no effect on an unlocked stack. 


## Examples

```
set the userModify of this stack to true

set the userModify of this stack to false
```

## Related Topics

* [cantModify](/HyperTalkReference/properties/cantModify)
