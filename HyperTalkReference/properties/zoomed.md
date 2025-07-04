---
title: zoomed
card_id: 79244
---

# zoomed

```
get [the] zoomed of [ph:window]
set [the] zoomed of [ph:window] to [ph:trueOrFalse]
```

When `the zoomed` is `true`, `[ph:window]` is full sized and centered on the current display. `The zoomed` becomes false when the user drags the window from its original position and/or resizes it.

`[ph:Window]` is any window with a zoom box.  If `[ph:window]` is straddling two displays, setting `the zoomed` to `true` opens `[ph:window]` to its full size and centers it on the display holding more than half  of the window's image.

Clicking the zoom box toggles `the zoomed` between true and false.

## Examples

```
get the zoomed of the card window
get the zoomed of window "My Picture"

set the zoomed of the card window to true
set the zoomed of window "Zoomer" to true
```

## Demo Script

```
on mouseUp
  set the <b>zoomed</b> of card window to true
  set the <b>zoomed</b> of card window to false
end mouseUp
```
