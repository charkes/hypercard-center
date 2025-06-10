---
title: suspendStack
card_id: 25274
---

# suspendStack

<code><pre>
suspendStack
</pre></code>

Handler:

<code><pre>
on suspendStack
  [ph:statements]
end suspendStack
</pre></code>

HyperCard sends the <code>suspendStack</code> message to the current card when the stack’s window becomes inactive (for example, when the user clicks another card window). 

HyperCard sends <code>suspendStack</code> only when it is displaying more than one stack. <code><pre>
</pre></code>

<code><b></code>Important</b>: HyperCard does not send <code>suspendStack</code> when the user switches to another layer under MultiFinder. (Click Related Topics for more information about the property<code> the suspended</code>.) 


## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
