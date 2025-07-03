---
title: enterInField
card_id: 36487
---

# enterInField

`enterInField`

HyperCard sends the `enterInField` command to a field when the user presses Enter and the insertion point is in the field.

This command saves the results of any changes the user or a handler makes to a field and closes the field.  

HyperCard sends a `closeField` message if the user made changes to the text or sends `exitField` if the user did not make any changes).

You can handle the `enterInField` message as follows:

```
on enterInField
  [ph:statements]
end enterInField
```

## Examples

```
Note the difference between these two scripts:

on addText
   select after text of bkgnd field "Example" -- set the insert point
   type "Hello world"  -- add some new text
   enterKey
end addText

on addText
   select after text of bkgnd field "Example" -- set the insert point
   type "Hello world"  -- add some new text
   enterInField
end addText

If you type addText into the Message box and press Return, the first script continually adds "Hello world" after existing text in the field. This is because the enterKey command sends the contents of the Message box—which in this case is addText—to the current card.

With the second script, addText places "Hello world" into the field once and then closes the field, saving the addition.
```

## Related Topics

* [closeField](/HyperTalkReference/systemmessages/closeField)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [newField](/HyperTalkReference/systemmessages/newField)
* [openField](/HyperTalkReference/systemmessages/openField)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
