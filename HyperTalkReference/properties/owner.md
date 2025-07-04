---
title: owner
card_id: 102019
---

# owner

```
get [the] [long|short] owner of [ph:card]
get [the] owner of [ph:window]
```

This read-only property tells you the  name of the background to which a specified card belongs, or it tells you the creator of a window.

`Long owner of [ph:card]` returns the full path name of the background. `Short owner of [ph:card]` returns the short name of the background.

`Owner of [ph:card]` returns “bkgnd” plus the leaf name of the background.

The `[ph:window]` form returns `HyperCard` if it's a stack or built-in window,  or the name of an XCMD if it's an external window.

## Examples

```
palette navigator
answer the owner of window "navigator" -- if it's showing

answer the owner of window "tools"

answer the short owner of card 1

answer "This card is in Background" && the short owner of this card
```
