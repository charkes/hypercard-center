---
title: clickChunk
card_id: 52836
---

# clickChunk

```
the clickChunk
```

Value returned: character chunk expression equal to the word the user clicked or the longest range of characters with the text style Group around the character that the user clicked (if the text has been grouped)  

The text style Group allows `the clickChunk` to extend beyond word boundaries.

The chunk expression returned has the following form:

```
char [ph:posInteger] to [ph:posInteger] ¬
     of [ph:container]
```

## Examples

```
put the clickChunk into theChunk
select theChunk

put the value of the clickChunk into theChunkClicked
put the textFont of the clickChunk into theFont
put the textStyle of the clickChunk into theStyle
```

## Demo Script

```
on clickDemo
  toggleActiveText true -- make sure grouped text is visible
  answer "Click any text in the Demo Script." & return & ¬
  "Click text with the gray underline (grouped text) to get phrases."
  wait until the mouseClick
  get the clickChunk
  select it
  wait 1 second
  answer "The chunk of text that you clicked was  “" & it & "”."
end clickDemo
```

## Related Topics

* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [selectedChunk](/HyperTalkReference/functions/selectedChunk)
* [show](/HyperTalkReference/commands/show)
* [textStyle](/HyperTalkReference/properties/textStyle)
