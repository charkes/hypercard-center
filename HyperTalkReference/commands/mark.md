---
title: mark
card_id: 41060
---

# mark

<code><pre>
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
</pre></code>

The <code>mark</code> command sets the <code>marked</code> property of the specified cards to <code>true</code>.  You can operate on the set of marked cards with commands such as <code>print</code>, <code>go</code>, <code>show</code>, and <code>sort</code>.

<code>Mark cards where</code> evaluates the given expression for every card in the stack. If its value is <code>true</code>, the card is marked.

<code>Mark cards by finding</code> marks cards using the same mechanism as the <code>find</code> command. It marks cards very quickly.

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
