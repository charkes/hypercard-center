---
title: unmark
card_id: 50277
---

# unmark

```
unmark all cards
unmark [ph:card]
unmark cards where [ph:trueOrFalse]
unmark cards by finding      ¬
  [chars|word|whole|string] ¬
  [international]           ¬
  [ph:text] [in [ph:field]] [of marked cards]
```

The `unmark` command sets the `marked` property of the specified cards to `false`.  Use it to deselect sets of cards that you have marked.

`Unmark cards where` visits each card in the stack and evaluates the expression. If its value is `true`, HyperCard unmarks the card. `Unmark cards by finding` unmarks cards using the same mechanism as the `find` command. It unmarks cards very quickly.

## Examples

```
unmark card
unmark this card
unmark first card
unmark first marked card
unmark marked card 12
unmark all cards

unmark cards where field "title" contains "select"
unmark cards where (word 2 of field "Pages" = 1)
unmark cards where isCommand() -- function returns true or false
unmark cards by finding "Mary Lou"
unmark cards by finding "Mary Lou" in field 1
-- unmark only some of the marked cards:
unmark cards by finding "Mary Lou" in field 1 of marked cards

-- This handler only unmarks the marked cards:

on unMarkCards
   repeat with i = 1 to the number of cards
     set cursor to busy
     if (the marked of card i) then unmark card i
   end repeat
end unMarkCards
```

## Related Topics

* [find](/HyperTalkReference/commands/find)
* [mark](/HyperTalkReference/commands/mark)
* [marked](/HyperTalkReference/properties/marked)
