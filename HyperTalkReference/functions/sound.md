---
title: sound
card_id: 64990
---

# sound

```
the sound
```

Value returned: a text string equal to the name of the sound resource currently playing (such as `"boing"`) or the string `"done"` if no sound is currently playing.

You use the `sound` function to synchronize sounds with other actions, because scripts continue to run while sounds are playing.

## Examples

```
if the sound is not done then ...

wait until the sound is done
```

## Related Topics

* [beep](/HyperTalkReference/commands/beep)
* [play](/HyperTalkReference/commands/play)
* [wait](/HyperTalkReference/commands/wait)
