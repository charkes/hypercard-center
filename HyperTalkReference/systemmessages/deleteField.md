---
title: deleteField
card_id: 19146
---

# deleteField

<code><pre>
deleteField
</pre></code>

Handler:

<code><pre>
on deleteField
  [ph:statements]
end deleteField
</pre></code>

HyperCard sends th<code>e deleteField </code>message to a field that is being deleted just before the field disappears. 

Note: You cannot stop a field from being deleted by trapping the <code>deleteField </code>message.  Instead, you must handle the <code>doMenu</code> message. 


## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
