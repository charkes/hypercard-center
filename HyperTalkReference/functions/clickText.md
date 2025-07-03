---
title: clickText
card_id: 53775
---

# clickText

```
the clickText
```

Value returned: text string equal to the word the user clicked  or the longest contiguous string of characters with the text style Group around the character that the user clicked

The text style Group allows `the clickText` to extend beyond word boundaries.

## Examples

```
put the clickText into theTextClicked

get the clickText
if it is not empty then go card it
```

## Demo Script

```
on clickDemo
  toggleActiveText true -- make sure grouped text is visible
  answer "Click any text in the Demo Script." & return & ¬
  "Click text with the gray underline (grouped text) to get phrases."
  wait until the mouseClick
  get the clickText
  select the clickChunk
  wait 1 second
  answer "The text that you clicked was  “" & it & "”."
end clickDemo
```

## Related Topics

* [show](/HyperTalkReference/commands/show)
* [textStyle](/HyperTalkReference/properties/textStyle)
