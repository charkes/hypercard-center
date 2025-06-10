---
title: closeField
card_id: 17449
modified: yes
---

# closeField

<code>closeField</code><br>
<br>
Handler:<br>
<br>
<code><pre>
on closeField
    <i>statements</i>
end closeField
</pre></code>

<br>
HyperCard sends the<code> closeField </code>message to an unlocked field when, after editing, a user (or handler) performs an action that closes (that is, removes the insertion point from) the field. HyperCard sends<code> closeField </code>only when the text actually changes.<br>
<br>
The following actions close a field, saving any changes that were made to the text:<br>
<br>
* Clicking outside the field<br>
* Moving the insertion point    to the next field with the Tab key<br>
* Pressing the Enter key<br>
* Pressing Command-Shift-Z to revert    the field to the last saved version<br>
* Going to another card<br>
* Quitting HyperCard<br>

## Placeholders

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
