---
title: visual
card_id: 50441
modified: yes
---

# visual

```
visual [effect] [ph:effect] [[ph:speed]] ¬
   [to [ph:image]]
```


The `visual` command specifies a visual effect for HyperCard to use as it moves from one card to another. (Click the placeholders `[ph:effect]`, `[ph:speed]`, and `[ph:image]` to see their possible replacements.) `Visual` must be followed by a `go` command to have any effect.

The optional `[ph:speed]` parameter tells HyperCard to perform the visual effect faster or slower than normal.

The `to [ph:image]` option changes the screen to white, gray, black, inverse, or the image of the destination card before applying the visual effect.

HyperCard uses the visual effect `plain` as its default effect. The default image is `card`.

Note: Only the effects `push`, `scroll`, `shrink`, `stretch`, and `zoom` work with the command `go this card`.

## Examples

```
visual zoom open
visual effect zoom open
visual effect zoom open fast
visual effect zoom open to black
visual effect zoom open very fast to black
```

## Demo Script

```
on mouseUp
 set cursor to watch
 set lockMessages to true -- leave the demo script up
 <b>visual</b> effect shrink to top to grey
 <b>visual</b> effect stretch from top to card
 go next card
 wait 10
 <b>visual</b> effect shrink to bottom slow to white
 <b>visual</b> effect stretch from top to card
 go prev card
 <b>visual</b> effect barn door close to black
 <b>visual</b> effect iris open slow to card
 go last card
 wait 10
 <b>visual</b> effect venetian blinds very slow
 go back
end mouseUp
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
