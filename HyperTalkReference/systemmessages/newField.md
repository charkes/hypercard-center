---
title: newField
card_id: 22421
---

# newField

```
newField
```

Handler:

```
on newField
  [ph:statements]
end newField
```

HyperCard sends the `newField` message to a field just after HyperCard creates it.

Although the new field will not have a script with which to respond to the message, any other object along the message-passing path can handle it.

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
