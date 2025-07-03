---
title: openField
card_id: 23457
---

# openField

```
openField
```

Handler:

```
on openField
  [ph:statements]
end openField
```

HyperCard sends the `openField` message to an unlocked field when a user (or handler) first opens it for text editing. A user opens a field for editing either by clicking in the field or by tabbing from the previous field.

Once opened for editing, a field no longer receives `openField` messages. 

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
