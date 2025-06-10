---
title: clickLoc
card_id: 53693
---

# clickLoc

<code><pre>
the clickLoc
</pre></code>

Value returned: [ph:<code>point] </code>equal to the place on the screen where the user most recently clicked relative to the top left corner of the current card

HyperCard does <b>not</b> reset <code>the clickLoc</code> at <code>idle,</code> nor does it reset when a handler is running, unless  you use the <code>wait</code> command: <code><pre>

wait until the mouseClick
</pre></code>


## Demo Script

<code><pre>
on mouseUp
  answer "Click anywhere on the screen."
  wait until the mouseClick
  answer "You clicked at" && the <b>clickLoc</b> &&¬
  "relative to the top left corner of the card."
end mouseUp
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouseLoc](/HyperTalkReference/functions/mouseLoc)
* [selectedLoc](/HyperTalkReference/functions/selectedLoc)
