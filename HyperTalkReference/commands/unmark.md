---
title: unmark
card_id: 50277
---

# unmark

<code><pre>
unmark all cards
unmark [ph:card]
unmark cards where [ph:trueOrFalse]
unmark cards by finding      ¬
  [chars|word|whole|string] ¬
  [international]           ¬
  [ph:text]
</pre></code>

[<code>in <i>field
</pre></code>

</i> ]  [<code>of marked cards
</pre></code>

] 

The <code>unmark</code> command sets the <code>marked</code> property of the specified cards to <code>false</code>.  Use it to deselect sets of cards that you have marked. <code><pre>
</pre></code>

<code>Unmark cards where </code>visits each card in the stack and evaluates the expression. If its value is <code>true</code>, HyperCard unmarks the card.<code> Unmark cards by finding</code> unmarks cards using the same mechanism as the <code>find</code> command. It unmarks cards very quickly. 


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
