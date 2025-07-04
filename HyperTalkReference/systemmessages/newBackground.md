---
title: newBackground
card_id: 21577
---

# newBackground

```
newBackground
```

Handler:

```
on newBackground
  [ph:statements]
end newBackground
```

HyperCard sends the `newBackground` message to the current card (in this case, the first card of the new background) just after HyperCard creates the background.

Although the new background will not have a script with which to respond to the message, any other object along the message-passing path can handle it. 

## Related Topics

* [closeBackground](/HyperTalkReference/systemmessages/closeBackground)
* [deleteBackground](/HyperTalkReference/systemmessages/deleteBackground)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [openBackground](/HyperTalkReference/systemmessages/openBackground)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
