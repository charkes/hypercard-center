---
title: cantDelete
card_id: 68822
---

# cantDelete

<code><pre>
set [the] cantDelete of [ph:card] ¬
   to [ph:trueOrFalse]
set [the] cantDelete of [ph:bkgnd] ¬
   to [ph:trueOrFalse]
set [the] cantDelete of [ph:stack] ¬
   to [ph:trueOrFalse]
</pre></code>

The <code>cantDelete</code> property returns or sets whether a user can delete a specified card, background, or stack. It corresponds to the Can’t Delete check box in the Card Info, Background Info, and Protect Stack dialog boxes. 

 The default value is <code>false</code> (meaning that a card, background, or stack can be deleted).

Note: Setting the <code>cantDelete</code> of a stack to <code>true</code> doesn't prevent the user from deleting the stack by dragging it to the Trash. 


## Examples

```
set the cantDelete of this card to true
set the cantDelete of first card of bkgnd 2 to false
set the cantDelete of this background to true
set the cantDelete of this stack to true
set the cantDelete of stack "Home" to true
```

## Demo Script

<code><pre>
on cantDeleteDemo
  set cantDelete of this card to true
  domenu "Delete Card"
end cantDeleteDemo
</pre></code>

## Related Topics

* [cantModify](/HyperTalkReference/properties/cantModify)
* [deleteBackground](/HyperTalkReference/systemmessages/deleteBackground)
* [deleteCard](/HyperTalkReference/systemmessages/deleteCard)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
