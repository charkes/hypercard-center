---
title: deleteButton
card_id: 18636
---

# deleteButton

```
deleteButton
```

Handler:

```
on deleteButton
  [ph:statements]
end deleteButton
```

HyperCard sends the `deleteButton` message to a button that is being deleted just before the button disappears.

Note:  You cannot stop a button from being deleted by trapping the `deleteButton` message. Instead, you must handle the `doMenu` message.

## Related Topics

* [doMenu](/HyperTalkReference/commands/doMenu)
* [newButton](/HyperTalkReference/systemmessages/newButton)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
