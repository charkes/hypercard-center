---
title: icon
card_id: 72855
---

# icon

`set `[`the`]` icon of [ph:button] ¬     to [ph:posInteger`] `set `[`the`]` icon of [ph:button] ¬     to [ph:text`]

where `[ph:text]` is the name of an icon.

The `icon` property returns or sets the icon displayed by a button. Setting it is the same as choosing an icon from the Button Info dialog box. HyperCard sets the function `the result` to `"Can't find that icon."` if it can’t find the icon (otherwise `the result` is` empty`). 

The value of the `icon` property is an integer corresponding to the ID number of an available icon resource. If a button has no icon, the `icon` property is 0. For an icon to be displayed on a button, its resource must be available in the current stack, one of the stacks currently being used, the Home stack, or HyperCard itself.

                          Click the goldfish bowl                           to see simple icon                           animations. 


## Examples

```
set the icon of bkgnd button "Prev" to 23875
set the icon of bkgnd button "Prev" to "Prev"

if the icon of button 1 is 34567 then ...
```

## Related Topics

* [result](/HyperTalkReference/functions/result)
