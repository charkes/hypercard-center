---
title: closeField
card_id: 17449
modified: yes
---

# closeField

`closeField`

Handler:

```
on closeField
    [ph:statements]
end closeField
```

HyperCard sends the `closeField` message to an unlocked field when, after editing, a user (or handler) performs an action that closes (that is, removes the insertion point from) the field. HyperCard sends `closeField` only when the text actually changes.

The following actions close a field, saving any changes that were made to the text:

* Clicking outside the field
* Moving the insertion point to the next field with the Tab key
* Pressing the Enter key
* Pressing Command-Shift-Z to revert the field to the last saved version
* Going to another card
* Quitting HyperCard

## Related Topics

* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
