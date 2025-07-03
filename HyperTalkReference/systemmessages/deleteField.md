---
title: deleteField
card_id: 19146
---

# deleteField

```
deleteField
```

Handler:

```
on deleteField
  [ph:statements]
end deleteField
```

HyperCard sends the `deleteField` message to a field that is being deleted just before the field disappears.

Note: You cannot stop a field from being deleted by trapping the `deleteField` message.  Instead, you must handle the `doMenu` message. 

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
