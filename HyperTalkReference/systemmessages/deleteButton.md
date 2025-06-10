---
title: deleteButton
card_id: 18636
---

# deleteButton

<code><pre>
deleteButton
</pre></code>

Handler:

<code><pre>
on deleteButton
  [ph:statements]
end deleteButton
</pre></code>

HyperCard sends th<code>e deleteButton </code>message to a button that is being deleted just before the button disappears. 

Note:  You cannot stop a button from being deleted by trapping the <code>deleteButton </code>message. Instead, you must handle the <code>doMenu</code> message. 


## Related Topics

* [doMenu](/HyperTalkReference/commands/doMenu)
* [newButton](/HyperTalkReference/systemmessages/newButton)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
