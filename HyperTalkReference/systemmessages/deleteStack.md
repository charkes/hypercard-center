---
title: deleteStack
card_id: 19234
---

# deleteStack

```
deleteStack
```

Handler:

```
on deleteStack
  [ph:statements]
end deleteStack
```

HyperCard sends the `deleteStack` message to the current card of the stack that is being deleted.

Note:  You cannot stop a stack from being deleted by trapping the `deleteStack` message. Instead, you must handle the `doMenu` message or set the `cantDelete` property for the stack. 

## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
