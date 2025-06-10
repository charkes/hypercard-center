---
title: deleteCard
card_id: 18888
---

# deleteCard

<code><pre>
deleteCard
</pre></code>

Handler:

<code><pre>
on deleteCard
  [ph:statements]
end deleteCard
</pre></code>

HyperCard sends the <code>deleteCard</code> message to a card that is being deleted just before the card disappears. 

Note:  You cannot stop a card from being deleted by trapping the <code>deleteCard </code>message. Instead, you must handle the <code>doMenu</code> message or set the <code>cantDelete</code> property for the card. 


## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeCard](/HyperTalkReference/systemmessages/closeCard)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newCard](/HyperTalkReference/systemmessages/newCard)
* [openCard](/HyperTalkReference/systemmessages/openCard)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
