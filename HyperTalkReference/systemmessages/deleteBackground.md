---
title: deleteBackground
card_id: 18315
modified: yes
---

# deleteBackground

<code><pre>
deleteBackground
</pre></code>

<br>
Handler:<br>
<br>
<code><pre>
on deleteBackground
    <i>statements</i>
end deleteBackground
</pre></code>

<br>
HyperCard sends the<code> deleteBackground </code>message to the card that is being deleted if no other cards in the stack share its background. HyperCard sends the message just before the card disappears.<br>
<br>
Note: You cannot stop a background from being deleted by trapping the <code>deleteBackground </code>message. Instead, you must handle the<code> doMenu </code>message or set the<code> cantDelete </code>property for the background.<br>

## Placeholders

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [closeBackground](/HyperTalkReference/systemmessages/closeBackground)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [newBackground](/HyperTalkReference/systemmessages/newBackground)
* [openBackground](/HyperTalkReference/systemmessages/openBackground)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
