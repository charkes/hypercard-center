---
title: dialingVolume
card_id: 99166
---

# dialingVolume

<code> set </code>[<code>the</code>]<code> dialingVolume to [ph:integer</code>]

The <code>dialingVolume</code> property sets or returns the volume of the dialing tones generated through the computer speaker by the <code>dial</code> command.

[ph:<code>integer] </code>evaluates to an integer in the range 0 through 7, where 0 is extremely low but does <u>not</u> shut off the sound entirely. 


## Examples

```
set dialingVolume to 5
if the dialingVolume is tooLoud then set the dialingVolume to 2
```

## Related Topics

* [dial](/HyperTalkReference/commands/dial)
* [dialingTime](/HyperTalkReference/properties/dialingTime)
