---
title: tabKey
card_id: 49516
---

# tabKey

`tabKey`

The `tabKey` command opens the first unlocked field on the current card or background (placing the insertion point in the field) and selects its entire contents.

If a field is already open for editing, `tabKey` closes it and opens the next editable field, selecting its contents. (A field is editable only if it is unlocked and visible.)

The `tabKey` command opens fields in the following order: from the lowest to the highest numbered background field, then from the lowest to the highest numbered card field.

HyperCard sends the `tabKey` command to a field or the current card when the user presses the Tab key. You can handle the `tabKey` message as follows:

```
on tabKey
  [ph:statements]
end tabKey
```

## Examples

```
-- Set the insertion point in the first editable field on openCard
on openCard  
   tabKey  
end openCard
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [enterKey](/HyperTalkReference/commands/enterKey)
* [returnKey](/HyperTalkReference/commands/returnKey)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
