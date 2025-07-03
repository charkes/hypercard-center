---
title: clickLoc
card_id: 53693
---

# clickLoc

```
the clickLoc
```

Value returned: `[ph:point]` equal to the place on the screen where the user most recently clicked relative to the top left corner of the current card

HyperCard does <b>not</b> reset `the clickLoc` at `idle`, nor does it reset when a handler is running, unless you use the `wait` command:

```
wait until the mouseClick
```

## Demo Script

```
on mouseUp
  answer "Click anywhere on the screen."
  wait until the mouseClick
  answer "You clicked at" && the <b>clickLoc</b> &&¬
  "relative to the top left corner of the card."
end mouseUp
```

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouseLoc](/HyperTalkReference/functions/mouseLoc)
* [selectedLoc](/HyperTalkReference/functions/selectedLoc)
