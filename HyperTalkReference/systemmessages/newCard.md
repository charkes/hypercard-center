---
title: newCard
card_id: 22221
---

# newCard

```
newCard
```

Handler:

```
on newCard
  [ph:statements]
end newCard
```

HyperCard sends the `newCard` message to the current card (in this case, the new one) just after HyperCard creates it.

Although the new card will not have a script with which to respond to the message, any other object along the message-passing path can handle it.

## Related Topics

* [closeCard](/HyperTalkReference/systemmessages/closeCard)
* [deleteCard](/HyperTalkReference/systemmessages/deleteCard)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [openCard](/HyperTalkReference/systemmessages/openCard)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
