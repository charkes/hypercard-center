---
title: longWindowTitles
card_id: 74508
---

# longWindowTitles

```
set the longWindowTitles ¬
   to [ph:trueOrFalse]
```

The `longWindowTitles` returns or sets whether HyperCard displays the full path name of a stack in the title bar of all windows that contain stacks. Its default value is false.

<b>WARNING:</b> Commands or properties that reference stack windows by name won't work once you set the `longWindowTitles` to true because the name becomes the full path name of a stack.

For example, compare the following two commands:

```
show window "Home"
show window "My HD:HyperCard:Home"
```

The first works only when the `longWindowTitles` is false, the second only when it's true. Check the value of the `longWindowTitles` before you use such commands or properties, or force it to be false in your stack (which takes away the feature).

## Examples

```
get the longWindowTitles

set the longWindowTitles to true
```

## Demo Script

```
on longWindowTitlesDemo
 set the cursor to watch
 set the <b>longWindowTitles</b> to not the <b>longWindowTitles</b>
 wait 2 second
 set the <b>longWindowTitles</b> to not the <b>longWindowTitles</b>
end longWindowTitlesDemo
```

## Related Topics

* [name](/HyperTalkReference/properties/name)
