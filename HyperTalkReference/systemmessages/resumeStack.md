---
title: resumeStack
card_id: 24386
---

# resumeStack

<code><pre>
resumeStack
</pre></code>

Handler:

<code><pre>
on resumeStack
  [ph:statements]
end resumeStack
</pre></code>

HyperCard sends the <code>resumeStack</code> message to the current card when the stack’s window becomes active after being inactive (for example, when the user clicks in a window). 

HyperCard sends<code> resumeStack </code>only when it is displaying more than one stack.

<b>Important</b>: HyperCard does not send <code>resumeStack</code> when the user switches to HyperCard from another layer under MultiFinder. (Click Related Topics for more information about the property<code> the suspended</code>.) 


## Related Topics

* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [startUp](/HyperTalkReference/systemmessages/startUp)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
