---
title: closeStack
card_id: 17907
modified: yes
---

# closeStack

`closeStack`

Handler:

```
on closeStack
    [ph:statements]
end closeStack
```

HyperCard sends the `closeStack` message to the current card when a user (or script) opens a different stack in the current window, closes the current window, deletes the stack, suspends HyperCard to launch an application, or quits HyperCard.

Note: If you have more than one stack open at a time, HyperCard sends `suspendStack`, not `closeStack`, when the stack becomes inactive.

## Placeholders

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
