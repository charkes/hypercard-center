---
title: The message-passing order
card_id: 8578
modified: yes
---

# The message-passing order

What happens if an object that receives a message <i>doesn’t</i> handle it?

In this case, HyperCard passes the message to other objects and searches their scripts for a message handler that matches the current message. The order in which HyperCard passes a message to objects is called the <i>message-passing order</i> or the <i>message-passing path</i>.

Initially, HyperCard sends messages to a specific button or field or to the current card. If a button or field doesn’t handle the message, it goes on to the current card. From the current card, the message goes to the following objects, in order:

* the current background
* the current stack
* the stack script of the Home stack
* HyperCard itself

## Related Topics

* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [pass](/HyperTalkReference/keywords/pass)
* [send](/HyperTalkReference/keywords/send)
* [start using](/HyperTalkReference/commands/start-using)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
