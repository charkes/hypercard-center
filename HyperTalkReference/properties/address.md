---
title: address
card_id: 102341
modified: yes
---

# address

<code>get the address</code>

This read-only property tells you where on the AppleTalk network you are, in the form<code> <i>zone</i>:<i>computer</i>:<i>program</i>.</code> If <code> <i>zone </i></code> is an asterisk (*), either your system is not on a network or the network has just one zone.

So if you're running HyperCard on a computer named Quille on a zone called HyperText,  the statement<code>  </code> <code>   put the address</code> yields       <code>HyperText:Quille:HyperCard</code>

If you're running HyperCard on an unnamed computer that's not on a network, you get

`*::HyperCard`

This property requires System 7.0 or later.

## Examples

```

put the address into cd fld "MyNetworkSpot"
```

## Placeholders

