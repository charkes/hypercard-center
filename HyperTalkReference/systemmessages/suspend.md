---
title: suspend
card_id: 25005
---

# suspend

`suspend`

Handler:

```
on suspend
  [ph:statements]
end suspend
```

HyperCard sends the `suspend` message to the current card when a user (or handler) launches an application from HyperCard with the `open` command, just before the application is launched.

Note: HyperCard does not send this message when it’s running under MultiFinder.

## Related Topics

* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [resume](/HyperTalkReference/systemmessages/resume)
* [suspended](/HyperTalkReference/properties/suspended)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
