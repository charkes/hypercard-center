---
title: foundChunk
card_id: 56033
---

# foundChunk

```
the foundChunk
```

Value returned: a character chunk expression that indicates where the most recent `find` command located its target string. If nothing was found, it returns `empty`. The chunk expression returned has the following form:

```
char [ph:posInteger] to [ph:posInteger] ¬
     of [ph:container]
```

## Examples

```
find "Maria"
put the foundChunk

--Using foundChunk to find and highlight a string:
find string userName in field "names"
select the foundChunk
```

## Demo Script

```
on foundChunkDemo
  find "foundChunkDemo" in field "Demo Script"
  get the <b>foundChunk</b> -- before select removes it
  wait 1 second
  select it
  answer "The foundChunk is:" & return & it
end foundChunkDemo
```

## Related Topics

* [clickChunk](/HyperTalkReference/functions/clickChunk)
* [find](/HyperTalkReference/commands/find)
* [selectedChunk](/HyperTalkReference/functions/selectedChunk)
