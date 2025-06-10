---
title: windows
card_id: 95475
---

# windows

<code><pre>
the windows
</pre></code>

Value returned: a return-separated list of the names of all the windows (including built-in palettes) in front-to-back order

If the <code>longWindowTitles</code> is true, <code>the windows</code> returns full path names for windows that contain stacks. 


## Examples

```
if "Home" & return is in the windows
then show window "Home" -- already open, just activate it
else go stack "Home"
```

## Demo Script

<code><pre>
on whatWindows
  answer "The windows are:" & return & return & the windows
end whatWindows
</pre></code>

