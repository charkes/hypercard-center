---
title: foundChunk
card_id: 56033
---

# foundChunk

<code><pre>
the foundChunk
</pre></code>

Value returned: a character chunk expression that indicates where the most recent <code>find</code> command located its target string. If nothing was found, it returns<code> empty</code>. The chunk expression returned has the following form:

<code>char</code> [ph:<code>posInteger] to [ph:posInteger] ¬     of [ph:container</code>] 


## Examples

```
find "Maria"
put the foundChunk

--Using foundChunk to find and highlight a string:
find string userName in field "names"
select the foundChunk
```

## Demo Script

<code><pre>
on foundChunkDemo
  find "foundChunkDemo" in field "Demo Script"
  get the <b>foundChunk</b> -- before select removes it
  wait 1 second
  select it
  answer "The foundChunk is:" & return & it
end foundChunkDemo
</pre></code>

## Related Topics

* [clickChunk](/HyperTalkReference/functions/clickChunk)
* [find](/HyperTalkReference/commands/find)
* [selectedChunk](/HyperTalkReference/functions/selectedChunk)
