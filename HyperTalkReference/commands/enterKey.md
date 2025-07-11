---
title: enterKey
card_id: 36714
---

# enterKey

`enterKey`

The `enterKey` command sends a statement typed into the Message box to the current card.

HyperCard sends the `enterKey` command to the current card when the user presses the Enter key unless the insertion point is in a field, in which case HyperCard sends` enterInField` instead.

You can handle the `enterKey` message as follows:

```
on enterKey
  [ph:statements]
end enterKey
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

If you type addText into the Message box and press Return, the first script continually adds "hello world" after existing text in the field. This is because the enterKey command sends the contents of the Message box—which in this case is addText—to the current card.

With the second script, addText places "Hello world" into the field once and then closes the field, saving the addition.
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
