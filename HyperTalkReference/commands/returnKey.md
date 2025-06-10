---
title: returnKey
card_id: 46524
---

# returnKey

<code><pre>
returnKey
</pre></code>

The <code>returnKey</code> command sends a statement typed into the Message box to the current card.

HyperCard sends the <code>returnKey</code> command to the current card when the user presses the Return key unless the insertion point is in a field, in which case HyperCard sends <code> returnInField </code>instead. 

You can handle the <code>returnKey</code> message as follows:

<code><pre>
on returnKey
  [ph:statements]
end returnKey
</pre></code>


## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [enterKey](/HyperTalkReference/commands/enterKey)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
