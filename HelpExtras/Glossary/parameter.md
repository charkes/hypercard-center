---
title: parameter
card_id: 19958
---

### parameter

A [g:value] passed to a handler as part of a message or function call.

Any expressions after the first word in a message are evaluated to yield the parameters to a message handler. For example, in the message

`myDisplay "Hello there world"`

the value of ` "Hello there world" `is the parameter passed to the `myDisplay` message handler.

Any expressions enclosed in parentheses are evaluated to yield the parameters to a function handler. For example, in the function call

`get totalValue(card field 1)`

the value of `card field 1` is the parameter passed to the `totalValue` function handler.

Multiple parameters are delimited by commas. 