---
title: pattern
card_id: 78411
modified: yes
---

# pattern

`set [the] pattern to [ph:posInteger]`

where `[ph:posInteger]` is an integer in the range 1 through 40.

The `pattern` property returns or sets the current pattern used to fill shapes or to paint with the Brush tool.

If you edit one of the patterns, HyperCard saves the new pattern with the stack.

[[image:%stack%/Card306.jpg]]

<i>Pattern IDs are organized from top to bottom and then left to right from 1 to 40. Top left is 1, bottom left is 10, top right is 31, bottom right is 40.</i>

## Examples

```
set the pattern to 1 -- white
set the pattern to 12 -- black
set the pattern to 22 -- gray
```

## Related Topics

* [brush](/HyperTalkReference/properties/brush)
* [lineSize](/HyperTalkReference/properties/lineSize)
* [reset](/HyperTalkReference/commands/reset)
