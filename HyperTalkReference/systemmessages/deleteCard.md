---
title: deleteCard
card_id: 18888
---

# deleteCard

```
deleteCard
```

Handler:

```
on deleteCard
  [ph:statements]
end deleteCard
```

HyperCard sends the `deleteCard` message to a card that is being deleted just before the card disappears.

Note:  You cannot stop a card from being deleted by trapping the `deleteCard` message. Instead, you must handle the `doMenu` message or set the `cantDelete` property for the card. 

## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeCard](/HyperTalkReference/systemmessages/closeCard)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newCard](/HyperTalkReference/systemmessages/newCard)
* [openCard](/HyperTalkReference/systemmessages/openCard)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
