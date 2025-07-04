---
title: address
card_id: 102341
modified: yes
---

# address

`get the address`

This read-only property tells you where on the AppleTalk network you are, in the form `[ph:zone]:[ph:computer]:[ph:program]`. If `[ph:zone]` is an asterisk (*), either your system is not on a network or the network has just one zone.

So if you're running HyperCard on a computer named Quille on a zone called HyperText,  the statement `put the address` yields `HyperText:Quille:HyperCard`

If you're running HyperCard on an unnamed computer that's not on a network, you get

`*::HyperCard`

This property requires System 7.0 or later.

## Examples

```
put the address into cd fld "MyNetworkSpot"
```

## Placeholders
