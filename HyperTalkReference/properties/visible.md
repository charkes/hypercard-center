---
title: visible
card_id: 88724
---

# visible

<code> set </code>[<code>the</code>]<code> visible of [ph:button] ¬     to [ph:trueOrFalse] set </code>[<code>the</code>]<code> visible of [ph:field] ¬     to [ph:trueOrFalse] set </code>[<code>the</code>]<code> visible of [ph:window] ¬     to [ph:trueOrFalse] set </code>[<code>the</code>]<code> visible of [ph:externalWindow] ¬     to [ph:trueOrFalse] set </code>[<code>the</code>]<code> visible of menuBar ¬     to [ph:trueOrFalse]

</code>The <code>visible</code> property returns or sets whether a button, field, window, or the menu bar is visible on the screen. 

 Setting the <code>visible</code> of a window to true makes it the frontmost window.

With external windows, an external command or external function must first create a window before the <code>visible</code> will work on it. <code></code>Setting the<code> visible</code> of a window to true (showing it) will <u>not</u> create the window. Similarly, setting the <code>visible</code> of a window to false (hiding it) doesn't remove it from the window list (from memory); use the <code>close</code> command to dispose of a window. 


## Examples

```
the visible of card button 1
the visible of bkgnd field id 34
the visible of message box
the visible of tool window
the visible of card window
the visible of message watcher
the visible of variable watcher

set the visible of bkgnd button "Next" to false
set the visible of card window to true
set the visible of field 1 to not (the visible of field 1)
```

## Demo Script

<code><pre>
on flashButton
  hideShowObject "bkgnd btn id 57", 6
end flashButton

on hideShowObject whatObject, howManyTimes
  repeat for (howManyTimes * 2) times
    set the <b>visible</b> of whatObject to not the <b>visible</b> of whatObject
  end repeat
end hideShowObject
</pre></code>

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [hide](/HyperTalkReference/commands/hide)
* [show](/HyperTalkReference/commands/show)
* [showPict](/HyperTalkReference/properties/showPict)
