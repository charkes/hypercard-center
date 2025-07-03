---
title: selectedChunk
card_id: 63264
---

# selectedChunk

```
the selectedChunk
```

Value returned: a character chunk expression that indicates the range of characters currently highlighted

If nothing is highlighted, `the selectedChunk` returns `empty`. The chunk expression returned has the following form:

```
char [ph:posInteger] to [ph:posInteger] ¬
     of [ph:container]
```

## Examples

```
get the selectedChunk

put the selectedChunk into theChunk
set the textStyle of theChunk to bold
```

## Demo Script

```
on selectedChunkDemo
   select text of field "Title"
   wait 15
   answer "The selectedChunk is:" & return & the selectedChunk
 end selectedChunkDemo
```

## Related Topics

* [clickChunk](/HyperTalkReference/functions/clickChunk)
* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [select](/HyperTalkReference/commands/select)
