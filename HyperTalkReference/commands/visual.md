---
title: visual
card_id: 50441
modified: yes
---

# visual

<code><pre>
visual [effect] <i>effect</i> [<i>speed</i>] ¬
   [to <i>image</i>]
</pre></code>


The<code> visual </code>command specifies a visual effect for HyperCard to use as it moves from one card to another. (Click the  placeholders<code> <i>effect</i>, <i>speed</i>,</code> and<code> <i>image</i> </code>to see their possible replacements.)<code> Visual</code> must be followed by a<code> go </code>command to have any effect.

The optional<code> <i>speed</i> </code>parameter tells HyperCard to perform the visual effect faster or slower than normal.

The<code> to <i>image</i> </code>option changes the screen to white, gray, black, inverse, or the image of the destination card before applying the visual effect.

HyperCard uses the visual effect<code> plain </code>as its default effect. The default image is<code> card</code>.

Note: Only the effects<code> push</code>, <code>scroll</code>,<code> shrink</code>,<code> stretch</code>, and<code> zoom</code>  work with the command<code> go this card</code>.

## Examples

```
visual zoom open
visual effect zoom open
visual effect zoom open fast
visual effect zoom open to black
visual effect zoom open very fast to black
```

## Demo Script

<code><pre>
<code><pre>
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
</pre></code>
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/effect.md]

[embed:HelpExtras/Placeholders/speed.md]

[embed:HelpExtras/Placeholders/image.md]

## Related Topics

* [go](/HyperTalkReference/commands/go)
