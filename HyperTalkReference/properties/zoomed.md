---
title: zoomed
card_id: 79244
---

# zoomed

<code><pre>
get [the] zoomed of [ph:window]
set [the] zoomed of [ph:window] ¬
   to [ph:trueOrFalse]
</pre></code>

When <code>the zoomed</code> is <code>true</code>,<code> [ph:window ]</code> is full sized and centered on the current display.<code> The zoomed </code>  becomes false when the user drags the window from its original position and/or resizes it. 

[ph: <code>Window</code>]  is any window with a zoom box.  If<code> [ph:window</code> ]is straddling two displays, setting <code>the zoomed</code> to <code>true</code> opens <code>[ph:window</code> ]to its full size and centers it on the display holding more than half  of the window's image.

Clicking the zoom box toggles <code>the zoomed</code> between true and false. 


## Examples

```
get the zoomed of the card window
get the zoomed of window "My Picture"

set the zoomed of the card window to true 
set the zoomed of window "Zoomer" to true
```

## Demo Script

<code><pre>
on mouseUp
  set the <b>zoomed</b> of card window to true
  set the <b>zoomed</b> of card window to false
end mouseUp
</pre></code>

