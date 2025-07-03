---
title: windows
card_id: 95475
---

# windows

```
the windows
```

Value returned: a return-separated list of the names of all the windows (including built-in palettes) in front-to-back order

If the `longWindowTitles` is true, `the windows` returns full path names for windows that contain stacks. 

## Examples

```
if "Home" & return is in the windows
then show window "Home" -- already open, just activate it
else go stack "Home"
```

## Demo Script

```
on whatWindows
  answer "The windows are:" & return & return & the windows
end whatWindows
```
