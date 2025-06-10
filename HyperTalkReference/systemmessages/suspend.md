---
title: suspend
card_id: 25005
---

# suspend

<code>suspend</code>

Handler:

<code><pre>
on suspend
  [ph:statements]
end suspend
</pre></code>

HyperCard sends the <code>suspend</code> message to the current card when a user (or handler) launches an application from HyperCard with the <code>open</code> command, just before the application is launched. 

Note: HyperCard does not send this message when it’s running under MultiFinder.

## Related Topics

* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [resume](/HyperTalkReference/systemmessages/resume)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
