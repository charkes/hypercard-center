---
title: openStack
card_id: 23747
---

# openStack

<code><pre>
openStack
</pre></code>

Handler:

<code><pre>
on openStack
  [ph:statements]
end openStack
</pre></code>

HyperCard sends the <code>openStack</code> message when a user (or handler) goes to a card in a stack different from that of the most recent card. 

Note: If you have more than one stack open at a time, HyperCard sends <code>resumeStack</code>, not<code> openStack</code>, when the stack becomes active. 


## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
