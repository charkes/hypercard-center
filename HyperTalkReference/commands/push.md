---
title: push
card_id: 45173
---

# push

```
push card
push [ph:card] [of [ph:stack]]
push [ph:bkgnd] [of [ph:stack]]
push [ph:stack]
```

The `push` command saves the identification of a card in HyperCard’s memory. If you specify a background or stack, HyperCard stores the location of the <b>first</b> card of the background or stack. In all cases, HyperCard saves the full card ID and the path name for the stack.

Each call to `push` saves a card ID in last-in, first-out order. You can return to saved locations using the `pop` command.

Note: The word `stack` that forms part of the stack identifier `[ph:stack]` is optional with the `push` command.

There is a limit of twenty pushes.

If you `pop` more than you `push`, you go to the Home stack.

## Examples

```
push card
push this card
push next card
push recent card -- remember where you've been
push card 234 of this stack

push first card of stack "Home"
push first card of "Home"

push background "Index" of stack "Glossary"
push background "Index" of "Glossary"

push stack "Home"
push "Home"
```

## Demo Script

```
on goHomeAndBack
  -- This demo shows that you can push and pop more than one card. Each
  -- successive pop goes back through the pushed cards.
  click at the loc of bkgnd button "close"
  set lockMessages to true
  <b>push</b> this card
  go prev card
  <b>push</b> this card
  wait 1 second
  go to card 3 of stack "Home"
  wait 1 second
  pop card
  pop card
  click at the loc of bkgnd button "Demo Script"
end goHomeAndBack
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [pop](/HyperTalkReference/commands/pop)
