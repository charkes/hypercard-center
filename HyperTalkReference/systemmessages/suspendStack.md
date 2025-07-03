---
title: suspendStack
card_id: 25274
---

# suspendStack

```
suspendStack
```

Handler:

```
on suspendStack
  [ph:statements]
end suspendStack
```

HyperCard sends the `suspendStack` message to the current card when the stack’s window becomes inactive (for example, when the user clicks another card window).

HyperCard sends `suspendStack` only when it is displaying more than one stack.

<code><b></code>Important</b>: HyperCard does not send `suspendStack` when the user switches to another layer under MultiFinder. (Click Related Topics for more information about the property `the suspended`.)


## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
