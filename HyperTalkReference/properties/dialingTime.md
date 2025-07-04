---
title: dialingTime
card_id: 98571
---

# dialingTime

`set [the] dialingTime to [ph:numberOfTicks]`

The `dialingTime` property sets or returns the total length of time (in ticks) that HyperCard leaves the serial port open while dialing a modem.

The default value for `[ph:numberOfTicks]` is 180, where 60 ticks = 1 second.

<b>Note</b>: `dialingTime` is <u>not</u> reset to its default value at idle time.

HyperCard maintains the value that you set for this property for the duration of the HyperCard session. 

## Related Topics

* [dial](/HyperTalkReference/commands/dial)
* [dialingVolume](/HyperTalkReference/properties/dialingVolume)
