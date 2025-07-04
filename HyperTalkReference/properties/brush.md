---
title: brush
card_id: 67958
modified: yes
---

# brush

<code>set [the] brush to <i>posInteger</i> </code>

where <i><code>posInteger</i></code> is a positive integer in the range 1 through 32.

The` brush `property returns or sets the current brush shape used by the Brush tool.

The value of the` brush `property represents a brush shape from the Brush Shape dialog box. The default brush is 8.

[[image:%stack%/Card254.jpg]]

<i>Brush IDs are organized top to bottom and then left to right from 1 to 32. Top left is 1, below top left is 2, etc. Second column starts with brush 5.</i>

## Examples

```
set the brush to 1
set the brush to 32
```

## Placeholders

[embed:HelpExtras/Placeholders/posInteger.md]

## Related Topics

* [lineSize](/HyperTalkReference/properties/lineSize)
* [pattern](/HyperTalkReference/properties/pattern)
* [reset](/HyperTalkReference/commands/reset)
