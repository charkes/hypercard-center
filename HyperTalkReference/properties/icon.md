---
title: icon
card_id: 72855
---

# icon

<code>set </code>[<code>the</code>]<code> icon of [ph:button] ¬     to [ph:posInteger</code>] <code>set </code>[<code>the</code>]<code> icon of [ph:button] ¬     to [ph:text</code>]

where <code>[ph:text]</code> is the name of an icon.

The <code>icon</code> property returns or sets the icon displayed by a button. Setting it is the same as choosing an icon from the Button Info dialog box. HyperCard sets the function <code>the result</code> to <code>"Can't find that icon."</code> if it can’t find the icon (otherwise <code>the result</code> is<code> empty</code>). 

The value of the <code>icon</code> property is an integer corresponding to the ID number of an available icon resource. If a button has no icon, the <code>icon</code> property is 0. For an icon to be displayed on a button, its resource must be available in the current stack, one of the stacks currently being used, the Home stack, or HyperCard itself.

                          Click the goldfish bowl                           to see simple icon                           animations. 


## Examples

```
set the icon of bkgnd button "Prev" to 23875
set the icon of bkgnd button "Prev" to "Prev"

if the icon of button 1 is 34567 then ...
```

## Related Topics

* [result](/HyperTalkReference/functions/result)
