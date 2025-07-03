---
title: beep
card_id: 31649
modified: yes
---

# beep

```
beep
beep [ph:posInteger]
```

The `beep` command sounds the Macintosh system beep.

If you specify a `[ph:posInteger]`, your Macintosh beeps that many times.

## Demo Script

```
on mouseUp
 <b>beep</b> 2
 answer "Beep! Beep!"
end mouseUp
```

## Placeholders

[embed:HelpExtras/Placeholders/posInteger.md]

## Related Topics

* [play](/HyperTalkReference/commands/play)
* [sound](/HyperTalkReference/functions/sound)
* [wait](/HyperTalkReference/commands/wait)
