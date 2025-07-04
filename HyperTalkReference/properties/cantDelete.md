---
title: cantDelete
card_id: 68822
---

# cantDelete

```
set [the] cantDelete of [ph:card] ¬
   to [ph:trueOrFalse]
set [the] cantDelete of [ph:bkgnd] ¬
   to [ph:trueOrFalse]
set [the] cantDelete of [ph:stack] ¬
   to [ph:trueOrFalse]
```

The `cantDelete` property returns or sets whether a user can delete a specified card, background, or stack. It corresponds to the Can’t Delete check box in the Card Info, Background Info, and Protect Stack dialog boxes. 

 The default value is `false` (meaning that a card, background, or stack can be deleted).

Note: Setting the `cantDelete` of a stack to `true` doesn't prevent the user from deleting the stack by dragging it to the Trash. 


## Examples

```
set the cantDelete of this card to true
set the cantDelete of first card of bkgnd 2 to false
set the cantDelete of this background to true
set the cantDelete of this stack to true
set the cantDelete of stack "Home" to true
```

## Demo Script

```
on cantDeleteDemo
  set cantDelete of this card to true
  domenu "Delete Card"
end cantDeleteDemo
```

## Related Topics

* [cantModify](/HyperTalkReference/properties/cantModify)
* [deleteBackground](/HyperTalkReference/systemmessages/deleteBackground)
* [deleteCard](/HyperTalkReference/systemmessages/deleteCard)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
