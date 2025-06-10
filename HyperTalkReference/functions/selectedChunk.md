---
title: selectedChunk
card_id: 63264
---

# selectedChunk

<code><pre>
the selectedChunk
</pre></code>

Value returned: a character chunk expression that indicates the range of characters currently highlighted

If nothing is highlighted, <code>the selectedChunk </code>returns<code> empty</code>. The chunk expression returned has the following form:

<code>char</code> [ph:<code>posInteger] to [ph:posInteger] ¬     of [ph:container</code>] 


## Examples

```
get the selectedChunk

put the selectedChunk into theChunk
set the textStyle of theChunk to bold
```

## Demo Script

<code><pre>
on selectedChunkDemo
   select text of field "Title"
   wait 15
   answer "The selectedChunk is:" & return & the selectedChunk
 end selectedChunkDemo
</pre></code>

## Related Topics

* [clickChunk](/HyperTalkReference/functions/clickChunk)
* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [select](/HyperTalkReference/commands/select)
