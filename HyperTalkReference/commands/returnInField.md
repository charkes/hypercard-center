---
title: returnInField
card_id: 46143
---

# returnInField

`returnInField`

The `returnInField` command places a return character at the position of the insertion point in a field.  

If the `autoTab` property of the field is `true` <i>and</i> the insertion point is on the last line of the field <i>and</i> the field is any type except scrolling, the `returnInField` command does not insert a return character but instead sends the `tabKey` command to the field.

HyperCard automatically sends the `returnInField` command to a field when the user presses Return and the insertion point is in the field.

You can handle the `returnInField` message as follows:

```
on returnInField
  [ph:statements]
end returnInField
```

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
