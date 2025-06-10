---
title: cursor
card_id: 70204
modified: yes
---

# cursor

<code>set [the] cursor to <i>cursor</i></code>

The<code> cursor </code>property sets the image that appears as the pointer on the screen.

<b>Note: </b><code>cursor</code> is a <code>set</code>-only property. You<b> </b>cannot<code> get </code>the current value of the<code> cursor </code>from a script.

HyperCard provides a number of built-in cursors that you can use. (HyperCard automatically resets the cursor to the image for the current tool on idle—when no other action is happening.)

The built-in cursors are:

* `Ibeam` (or `1`)
* `cross` (or `2`)
* `plus` (or `3`)
* `watch` (or `4`)
* `hand`
* `arrow`
* `busy`
* `none`

The<code> busy </code>cursor rotates an eighth of a turn each time you call it.

## Examples

```
set the cursor to 1
set the cursor to 4
set the cursor to Ibeam
set the cursor to none
set the cursor to watch

repeat with i = 1 to 100
  set the cursor to busy -- spins the beach ball
  ...
end repeat
```

## Demo Script

<code><pre>
on rotateCursors
  repeat with cursorNumber = 1 to 4
    set the <b>cursor</b> to cursorNumber
    wait 30
  end repeat
  set the <b>cursor</b> to hand
  wait 30
  set the <b>cursor</b> to arrow
  wait 30
  set the <b>cursor</b> to balloon -- a cursor in the HyperCard Help stack
  wait 30
  repeat for 73
    set the <b>cursor</b> to busy
    wait 1
  end repeat
end rotateCursors
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/cursor.md]

