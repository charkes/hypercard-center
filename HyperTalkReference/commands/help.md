---
title: help
card_id: 39675
---

# help

`help`

The `help` command goes to the first card of the HyperCard Help stack.

HyperCard sends the `help` command to the current card when the user chooses Help from the Go menu (or presses Command-?).

Note: The command `go help` is equivalent to `go stack "help"`, while the `help` command tries to execute `go stack "HyperCard Help"`.

You can handle the `help` message as follows:

```
on help
  [ph:statements]
end help
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
