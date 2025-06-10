---
title: sort
card_id: 48321
modified: yes
---

# sort

<code><pre>
sort [<i>sortDirection</i>] [<i>sortStyle</i>] ¬
   by <i>expression</i>

sort [this] stack [<i>sortDirection</i>] ¬
   [<i>sortStyle</i>] by <i>expression</i>

sort [marked] cards [of this stack] ¬
   [<i>sortDirection</i>] [<i>sortStyle</i>] ¬
   by <i>expression</i>

sort <i>bkgnd</i> [<i>sortDirection</i>] ¬
   [<i>sortStyle</i>] by <i>expression</i>

sort [marked] cards of <i>bkgnd</i> ¬
   [<i>sortDirection</i>] [<i>sortStyle</i> ] ¬
   by <i>expression</i>

sort [<i>chunks</i> of] <i>container</i> ¬
   [<i>sortDirection</i>] [<i>sortStyle</i>] ¬
   [by <i>expression</i>]
</pre></code>


where<code> <i>chunks</i> </code>are limited to either lines or items.

The first five forms of the<code> sort </code>command order all the cards in a stack or background by the value of<code> <i>expression</i>,</code> evaluated  for each card in the stack or background.

The last form of the<code> sort </code>command (<code>by <i>expression</i></code> )<code> </code>sorts lines or items of a container by any expression. If you don’t specify,<code> sort </code>orders by lines.  Before<code> <i>expression</i> </code>is evaluated for each line or item of the container, the local variable<code> each </code>is set to the contents of the chunk. (Click the Examples button to see syntax examples using<code> each</code>.)

For all forms of the<code> sort </code>command, the default sort direction is<code> ascending, </code>and the default sort style is<code> text</code>.

Sort direction<code> ascending </code>orders the sort elements—the value of the expression on each card or the lines or items in the container—from lower to higher values.

Sort direction<code> descending </code>orders the sort elements from higher to lower values.

Sort style<code> text </code>compares the sort elements based on their ASCII values:

<code>"1" < "101" < "2" < "a" < "ab" < "b"</code>

Note that neither case nor diacritical marks matter with the sort style<code> text</code>:

`"apple" = "APPLE" = "äpplé"`

Sort style<code> numeric </code>correctly sorts numbers.  With sort style<code> text,</code>

`"1" < "100" < "17" < "2"`

The sort style<code> numeric </code>correctly sorts these values as:

<code>"1" < "2" < "17" < "100"</code>

The sort style<code> dateTime </code>orders the sort elements by their date or time format. (See the<code> convert </code>command for valid date and time formats.)

The sort style<code> international </code>correctly sorts non-English text containing diacritical marks and special characters based on the international resource installed in the current stack, the Home stack, HyperCard itself, or the System file.

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

<code><pre>
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
Harpo<b>
</b>
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/sortDirection.md]

[embed:HelpExtras/Placeholders/sortStyle.md]

[embed:HelpExtras/Placeholders/expression.md]

[embed:HelpExtras/Placeholders/bkgnd.md]

[embed:HelpExtras/Placeholders/chunks.md]

[embed:HelpExtras/Placeholders/container.md]

## Related Topics

* [mark](/HyperTalkReference/commands/mark)
