---
title: newStack
card_id: 22569
---

# newStack

<code><pre>
newStack
</pre></code>

Handler:

<code><pre>
on newStack
  [ph:statements]
end newStack
</pre></code>

HyperCard sends the <code>newStack</code> message to the current card (in this case, the first card of the new stack) just after HyperCard creates the stack. 

Although the new stack will not have a script with which to respond to the message, any other object along the message-passing path can handle it. 


## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
