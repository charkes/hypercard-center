---
title: beep
card_id: 31649
modified: yes
---

# beep

<code><pre>
beep
beep [ph:posInteger]
</pre></code>


The <code>beep</code> command sounds the Macintosh system beep.

If you specify a <code>[ph:posInteger]</code>, your Macintosh beeps that many times.

## Demo Script

<code><pre>
on mouseUp
 <b>beep</b> 2
 answer "Beep! Beep!"
end mouseUp
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/posInteger.md]

## Related Topics

* [play](/HyperTalkReference/commands/play)
* [sound](/HyperTalkReference/functions/sound)
* [wait](/HyperTalkReference/commands/wait)
