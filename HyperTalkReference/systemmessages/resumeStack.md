---
title: resumeStack
card_id: 24386
---

# resumeStack

```
resumeStack
```

Handler:

```
on resumeStack
  [ph:statements]
end resumeStack
```

HyperCard sends the `resumeStack` message to the current card when the stack’s window becomes active after being inactive (for example, when the user clicks in a window).

HyperCard sends `resumeStack` only when it is displaying more than one stack.

<b>Important</b>: HyperCard does not send `resumeStack` when the user switches to HyperCard from another layer under MultiFinder. (Click Related Topics for more information about the property `the suspended`.)

## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [startUp](/HyperTalkReference/systemmessages/startUp)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
