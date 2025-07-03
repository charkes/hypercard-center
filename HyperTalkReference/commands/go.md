---
title: go
card_id: 38981
modified: yes
---

# go

```
go [to] [ph:ordinal]
go [to] [ph:position]
go [to] [ph:card] [of [ph:bkgnd]] [of [ph:stack]]
go [to] [ph:bkgnd] [of [ph:stack]]
go [to] [ph:stack]
go [to] [[ph:card] of] [[ph:bkgnd] of] [ph:stack] ¬
   [in a new window] [without dialog]
```


The `go` command takes the user to a card in a stack. The `[ph:ordinal]` and `[ph:position]` forms take the user to a card in the current stack.

If you name a stack (or background) without specifying a card, HyperCard goes to the first card of the stack (or background).

HyperCard puts `empty` into the function `the result` when the `go` command succeeds; it puts `"No such card."` or `"No such stack."` into `the result` when it can’t go to the card or stack.

The `in a new window` option tells HyperCard to open a stack in another window when it goes to the stack.

The `without dialog` option tells HyperCard to go to another stack directly based on the search paths that are specified on the Search Paths card of the user’s Home stack. If HyperCard can't find the stack, it places `"No such stack"` into `the result`.

If you don't use `without dialog`, `the result` is set to `Cancel` if the user clicks the "Where Is" dialog box's Cancel button.

Note: The options `in a new window` and `without dialog` take effect only if the `go` command explicitly specifies a stack other than the current stack.

## Examples

```
--Go to an ordinal in the current stack (referring to cards):
go first
go last
go second
go third

--Go to a position in the current stack (referring to cards):
go this
go next
go prev

-- Go to a different card, perhaps in a different stack:
go back -- could be in another stack
go forth -- could be in another stack
go card 4
go card id 23405
go first card
go next card
go previous card
go recent card -- could be in another stack
go last card
go mid card
go any card
go first card of bkgnd 2
go card 1 of second bkgnd of stack "My Stack"

-- Go to a different background in the current stack:
go bkgnd "Index"
go bkgnd "Index" of stack "My Stack"

-- Go to a different stack:
go to stack "Address"
go stack "Address"
go "Address"
go home  
go help

-- Use full pathname:
go "Simonides:Fly II:Current Fly:Help"

-- Go to new stack, but open it in a new window:
go stack "My Stack" in a new window
if the result is not empty then ... -- couldn't open it in a new window

-- Go to a new stack, but skip the dialog asking where the stack is if -- HyperCard can't find it:
go stack "My Stack" without dialog
if the result is not empty then ... -- didn't go there

-- Go to a new stack,open it in a new window, and skip the dialog:
go to stack "Home" in new window without dialog
```

## Demo Script

```
on goFirstCardAndBack
  set cursor to watch
  set lockMessages to true -- to leave the demo script up
  <b>go</b> first card
  <b>go</b> back
end goFirstCardAndBack
```

## Placeholders

[embed:HelpExtras/Placeholders/ordinal.md]

[embed:HelpExtras/Placeholders/position.md]

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/bkgnd.md]

[embed:HelpExtras/Placeholders/stack.md]

## Related Topics

* [lock](/HyperTalkReference/commands/lock)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
* [mark](/HyperTalkReference/commands/mark)
* [pop](/HyperTalkReference/commands/pop)
* [push](/HyperTalkReference/commands/push)
* [unlock](/HyperTalkReference/commands/unlock)
* [visual](/HyperTalkReference/commands/visual)
