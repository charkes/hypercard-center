---
title: handler
card_id: 14222
---

### handler

A block of HyperTalk statements, contained in the [g:script] of an object, that executes in response to a message or a function call matching the handler’s name.

The first line in a handler must begin with the keywords `on` or `function` followed by the name of the message or function. The last line of the handler must end with the keyword` end`.

Handlers defined using the `on` keyword are called[ph: message handlers.]  You use a message handler to respond to messages sent by HyperCard or your scripts.

Handlers defined using the `function` keyword are called[ph: function handlers ]. You use function handlers to return a value to the handler that calls it. 