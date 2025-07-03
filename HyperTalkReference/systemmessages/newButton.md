---
title: newButton
card_id: 21952
---

# newButton

```
newButton
```

Handler:

```
on newButton
  [ph:statements]
end newButton
```

HyperCard sends the `newButton` message to a button just after HyperCard creates it.

Although the new button will not have a script with which to respond to the message, any other object along the message-passing path can handle it. 

## Examples

```
--This handler sets the autoHilite for each new button:

on newButton
  -- the target is the name of the new button
  set autoHilite of the target to true
  pass newButton
end newButton
```

## Related Topics

* [deleteButton](/HyperTalkReference/systemmessages/deleteButton)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
