---
title: deleteStack
card_id: 19234
---

# deleteStack

<code><pre>
deleteStack
</pre></code>

Handler:

<code><pre>
on deleteStack
  [ph:statements]
end deleteStack
</pre></code>

HyperCard sends the <code>deleteStack</code> message to the current card of the stack that is being deleted. 

Note:  You cannot stop a stack from being deleted by trapping the <code>deleteStack </code>message. Instead, you must handle the <code>doMenu</code> message or set the <code>cantDelete</code> property for the stack. 


## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
