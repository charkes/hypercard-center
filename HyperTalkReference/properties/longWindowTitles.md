---
title: longWindowTitles
card_id: 74508
---

# longWindowTitles

<code><pre>
set the longWindowTitles ¬
   to <i>trueOrFalse
</pre></code>

</i>

The <code>longWindowTitles</code> returns or sets whether HyperCard displays the full path name of a stack in the title bar of all windows that contain stacks. Its default value is false.

<b>WARNING: </b>Commands or properties that reference stack windows by name won't work once you set the <code>longWindowTitles</code> to true because the name becomes the full path name of a stack. 

For example, compare the following two commands:

<code><pre>
show window "Home"
show window "My HD:HyperCard:Home"
</pre></code>

The first works only when the<code> longWindowTitles</code> is false, the second only when it's true. Check the value of the<code> longWindowTitles</code> before you use such commands or properties, or force it to be false in your stack (which takes away the feature). 


## Examples

```
get the longWindowTitles

set the longWindowTitles to true
```

## Demo Script

<code><pre>
<code><pre>
on longWindowTitlesDemo
 set the cursor to watch
 set the <b>longWindowTitles</b> to not the <b>longWindowTitles</b>
 wait 2 second
 set the <b>longWindowTitles</b> to not the <b>longWindowTitles</b>
end longWindowTitlesDemo
</pre></code>
</pre></code>

## Related Topics

* [name](/HyperTalkReference/properties/name)
