---
title: deleteBackground
card_id: 18315
modified: yes
---

# deleteBackground

```
deleteBackground
```

Handler:

```
on deleteBackground
    [ph:statements]
end deleteBackground
```

HyperCard sends the `deleteBackground` message to the card that is being deleted if no other cards in the stack share its background. HyperCard sends the message just before the card disappears.

Note: You cannot stop a background from being deleted by trapping the `deleteBackground` message. Instead, you must handle the `doMenu` message or set the `cantDelete` property for the background.

## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeBackground](/HyperTalkReference/systemmessages/closeBackground)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newBackground](/HyperTalkReference/systemmessages/newBackground)
* [openBackground](/HyperTalkReference/systemmessages/openBackground)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
