---
title: tabKey
card_id: 49516
---

# tabKey

<code>tabKey</code>

The <code>tabKey</code> command opens the first unlocked field on the current card or background (placing the insertion point in the field) and selects its entire contents.

If a field is already open for editing, <code>tabKey</code> closes it and opens the next editable field, selecting its contents. (A field is editable only if it is unlocked and visible.)

The <code>tabKey</code> command opens fields in the following order: from the lowest to the highest numbered background field, then from the lowest to the highest numbered card field.

HyperCard sends the <code>tabKey</code> command to a field or the current card when the user presses the Tab key. You can handle the <code>tabKey</code> message as follows:

<code><pre>
on tabKey
  [ph:statements]
end tabKey
</pre></code>

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
