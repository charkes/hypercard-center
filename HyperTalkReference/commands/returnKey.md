---
title: returnKey
card_id: 46524
---

# returnKey

```
returnKey
```

The `returnKey` command sends a statement typed into the Message box to the current card.

HyperCard sends the `returnKey` command to the current card when the user presses the Return key unless the insertion point is in a field, in which case HyperCard sends `returnInField` instead.

You can handle the `returnKey` message as follows:

```
on returnKey
  [ph:statements]
end returnKey
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [enterKey](/HyperTalkReference/commands/enterKey)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
