---
title: mark
card_id: 41060
---

# mark

```
mark all cards
mark [ph:card]
mark cards where [ph:trueOrFalse]
mark cards by finding ¬
       [international] [ph:text] [in [ph:field]]
mark cards by finding chars ¬
     [international] [ph:text] [in [ph:field]]
mark cards by finding word ¬
     [international] [ph:text] [in [ph:field]]
mark cards by finding whole ¬
     [international] [ph:text] [in [ph:field]]
mark cards by finding string ¬
     [international] [ph:text] [in [ph:field]]
```

The `mark` command sets the `marked` property of the specified cards to `true`.  You can operate on the set of marked cards with commands such as `print`, `go`, `show`, and `sort`.

`Mark cards where` evaluates the given expression for every card in the stack. If its value is `true`, the card is marked.

`Mark cards by finding` marks cards using the same mechanism as the `find` command. It marks cards very quickly.

## Examples

```
mark all cards

mark card 1
mark any card
mark last card of next bkgnd

mark cards where field "title" contains "select"
mark cards where (word 2 of field "Pages" = 1)
mark cards where isaCommand() -- a function that returns true or false

mark cards by finding "Duffy" in bkgnd field "Author"
mark cards by finding whole "Cupertino, CA" in field "Address"
mark cards by finding international "schøål" in field 5
```

## Related Topics

* [find](/HyperTalkReference/commands/find)
* [go](/HyperTalkReference/commands/go)
* [marked](/HyperTalkReference/properties/marked)
* [print](/HyperTalkReference/commands/print)
* [show](/HyperTalkReference/commands/show)
* [sort](/HyperTalkReference/commands/sort)
* [unmark](/HyperTalkReference/commands/unmark)
