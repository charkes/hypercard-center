---
title: returnInField
card_id: 46143
---

# returnInField

<code>returnInField</code>

The <code>returnInField</code> command places a return character at the position of the insertion point in a field.  

If the <code>autoTab</code> property of the field is <code>true</code> <i>and</i> the insertion point is on the last line of the field <i>and</i> the field is any type except scrolling, the <code>returnInField</code> command does not insert a return character but instead sends the <code>tabKey</code> command to the field.

HyperCard automatically sends the <code>returnInField</code> command to a field when the user presses Return and the insertion point is in the field.

You can handle the <code>returnInField</code> message as follows:

<code><pre>
on returnInField
  [ph:statements]
end returnInField
</pre></code>

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
