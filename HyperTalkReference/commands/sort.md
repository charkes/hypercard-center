---
title: sort
card_id: 48321
modified: yes
---

# sort

```
sort [[ph:sortDirection]] [[ph:sortStyle]] ¬
   by [ph:expression]

sort [this] stack [[ph:sortDirection]] ¬
   [[ph:sortStyle]] by [ph:expression]

sort [marked] cards [of this stack] ¬
   [[ph:sortDirection]] [[ph:sortStyle]] ¬
   by [ph:expression]

sort [ph:bkgnd] [[ph:sortDirection]] ¬
   [[ph:sortStyle]] by [ph:expression]

sort [marked] cards of [ph:bkgnd] ¬
   [[ph:sortDirection]] [[ph:sortStyle] ] ¬
   by [ph:expression]

sort [[ph:chunks] of] [ph:container] ¬
   [[ph:sortDirection]] [[ph:sortStyle]] ¬
   [by [ph:expression]]
```

where `[ph:chunks]` are limited to either lines or items.

The first five forms of the `sort` command order all the cards in a stack or background by the value of `[ph:expression]`, evaluated for each card in the stack or background.

The last form of the `sort` command (`by [ph:expression]` ) sorts lines or items of a container by any expression. If you don’t specify, `sort`orders by lines.  Before `[ph:expression]` is evaluated for each line or item of the container, the local variable `each` is set to the contents of the chunk. (Click the Examples button to see syntax examples using `each`.)

For all forms of the `sort` command, the default sort direction is `ascending,` and the default sort style is `text`.

Sort direction `ascending` orders the sort elements—the value of the expression on each card or the lines or items in the container—from lower to higher values.

Sort direction `descending` orders the sort elements from higher to lower values.

Sort style `text` compares the sort elements based on their ASCII values:

`"1" < "101" < "2" < "a" < "ab" < "b"`

Note that neither case nor diacritical marks matter with the sort style `text`:

`"apple" = "APPLE" = "äpplé"`

Sort style `numeric` correctly sorts numbers. With sort style `text`,

`"1" < "100" < "17" < "2"`

The sort style `numeric` correctly sorts these values as:

`"1" < "2" < "17" < "100"`

The sort style `dateTime` orders the sort elements by their date or time format. (See the `convert` command for valid date and time formats.)

The sort style `international` correctly sorts non-English text containing diacritical marks and special characters based on the international resource installed in the current stack, the Home stack, HyperCard itself, or the System file.

## Examples

```
-- Sort a container:

sort lines of card field 1
sort items of card field 1
sort lines of myVariable descending numeric
sort items of Message box
sort lines of the selection
sort lines of field 1 by last word of each -- by last word of each line
sort items of fld 1 descending numeric by word 2 of each
sort items of myList by the random of 2000 -- reorder myList randomly
sort lines of fld 1 numeric by length(cd fld each) -- if field 1
            -- contains names of cd flds, orders names according
            -- to number of characters in each field.

-- Sort cards:

sort by bkgnd field "Name"
sort this stack by bkgnd field "Name"
sort stack by bkgnd field "Name"
sort marked cards of this stack by bkgnd field "Name"

sort this background by bkgnd field "Name"
sort background 2 by bkgnd field "Name"
sort marked cards of previous background by bkgnd field "Name"

sort descending by bkgnd field "Name"
sort descending international by bkgnd field "Name"

sort numeric by bkgnd field 2
sort numeric by the id of this card

sort by (bkgnd field "Last Name" & bkgnd field "First Name")
sort by mySortFunction()
```

## Demo Script

```
on sortMe
  put line 10 to 13 of me into theLines
  select line 10 to 13 of me
  wait 30
  sort lines of the selection
  wait 1 second
  put theLines into line 10 to 13 of me
end sortMe

Zeppo
Chico
Groucho
Harpo
```

## Related Topics

* [mark](/HyperTalkReference/commands/mark)
