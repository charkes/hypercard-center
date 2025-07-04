---
title: find
card_id: 37172
modified: yes
---

# find

```
find [international] [ph:text ] ¬
   [in [ph:field]] [of marked cards]

find chars [international] [ph:text] ¬
   [in [ph:field]] [of marked cards]

find word [international] [ph:text] ¬
   [in [ph:field]] [of marked cards]

find whole [international] [ph:text] ¬
   [in [ph:field]] [of marked cards]

find string [international] [ph:text] ¬
   [in [ph:field]] [of marked cards]
```


The `find` command searches for a text string in <b>all</b> the card and background fields (visible or not) of the current stack.

`International` considers diphthongs and diacritical marks as it searches. `In [ph:field]`searches only a specific card or background field. `Of marked cards` restricts its search to marked cards.

When `find` succeeds, a box appears around found text (or the first part of the text if the targets are discontinuous); `the result` is set to `empty`. When `find` fails, `the result` is set to the string `"Not found"`.

The commands `find`, `find chars`, and `find word` treat each word of the search string as a separate search item. For example, `find "this command"` is treated as `find "this"` <b>and</b> `find "command"`. The search succeeds if HyperCard finds all the words of the search string <b>anywhere</b> on the card (or anywhere in the specified field). The words do not have to be in order.

The commands `find whole` and `find string` treat spaces as part of the search string. For example, `find whole "this command"` succeeds only if HyperCard finds that exact string, including the space. The words must appear in order for `find whole` to succeed.

To prevent find from searching in a particular field, card, or background, see `dontSearch` in Related Topics.

Here are the forms of `find` types:

* find: Whole or partial strings starting from the beginning of a word.

* find chars: Partial strings anywhere within a word.

* find word: Whole words only.

* find whole: Whole or partial strings, including spaces, starting from the beginning of a word.

* find string: Partial strings anywhere, including spaces (ignores word boundaries).

## Examples

```
find "HyperCard"

-- Restrict the search:
find "select" in bkgnd field "Title"
find "select" in card field id 8293
find "select" in marked cards
find "select" in field 2 of marked cards

-- Find partial matches or whole words only:
find chars "elect" in bkgnd fld "title" -- will match select
find word "msg" in second card field  
find chars international "bøhr"

-- Find whole and find string include any spaces as part of the string:
find whole "lets you search for a whole phrase"
find string "ets you search for part of a phr"

-- Find the contents of a variable:
find whole currentFindVar

-- Find the contents of a field:
find whole (field "title") in field "index"

-- Find any general expression:
find string (char 1 to 4 of the short name of this card)
```

## Demo Script

```
on findDemo
 -- find a contiguous string of characters, including spaces:
  set cursor to watch
  <b>find string</b> "ind a contig" in field "Demo Script"
  wait 2 seconds
  -- next, find a phrase:
  <b>find whole</b> "find a phrase" in field "Demo Script"
  wait 2 seconds
end findDemo
```

## Related Topics

* [dontSearch](/HyperTalkReference/properties/dontSearch)
* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [foundField](/HyperTalkReference/functions/foundField)
* [foundLine](/HyperTalkReference/functions/foundLine)
* [foundText](/HyperTalkReference/functions/foundText)
* [mark](/HyperTalkReference/commands/mark)
