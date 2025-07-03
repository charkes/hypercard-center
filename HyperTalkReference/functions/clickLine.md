---
title: clickLine
card_id: 53252
---

# clickLine

```
the clickLine
```

Value returned: line chunk expression equal to the line that the user  clicked or, if the text has been grouped,  the first line of the longest range of lines with the text style Group around the character that the user clicked

The text style Group allows `the clickLine` to extend beyond one line.

The chunk expression returned has the following form:

`line [ph:posInteger] of [ph:container]` 

## Examples

```
put the clickLine into theLine
select theLine

put the value of the clickLine into theLineClicked
put the textFont of the clickLine into theFont
put the textStyle of the clickLine into theStyle
```

## Demo Script

```
on clickDemo
  answer "Click any line of the Demo Script."
  wait until the mouseClick
  get the <b>clickLine</b>
  select it
  wait 1 second
  answer "The clickline is:" & return & it & return
end clickDemo
```

## Related Topics

* [foundLine](/HyperTalkReference/functions/foundLine)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
* [show](/HyperTalkReference/commands/show)
* [textStyle](/HyperTalkReference/properties/textStyle)
