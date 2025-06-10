---
title: hide
card_id: 39797
modified: yes
---

# hide

<code><pre>
hide menuBar
hide titleBar
hide groups
hide card picture
hide background picture
hide picture of <i>card</i>
hide picture of <i>bkgnd</i>
hide <i>field</i>
hide <i>button</i>
hide <i>window</i>
hide <i>externalWindow</i>
</pre></code>


The <code>hide</code> command removes HyperCard objects and elements from view.

<code>hide menuBar</code> removes the menu bar from the top of the screen.

<code>hide titleBar</code> removes the title bar on the card window.

Use both of these commands with care: hiding the menu bar, or the title bar of a window, may confuse your users.

The hide groups command removes the two-pixel gray underline displayed for all text that has the “group” text style. The underline appears only after a show groups command.

For graphics, the hide command removes the card or background picture from view. It’s the same as setting the showPict property of the card or background to false.

For buttons, fields, and windows, the `hide` command is equivalent to setting the `visible` property to `false`.

If you hide the frontmost document window, the next document window becomes active. `Hide` does not remove an external window from the window list (from memory); use the `close` command to dispose of the window.

## Examples

```
hide card window

-- built-in windows:
hide tool window
hide window "tools"
hide Message box
hide window "Message"
hide message watcher
hide window "Message Watcher"
hide variable watcher
hide window "Variable Watcher"

-- external windows:
hide window "Navigator"
hide window "Script of My HD:Home"

hide button 1
hide second bkgnd field

hide picture of card 3
hide pict of first cd
hide picture of background "jazz"
```

## Demo Script

<code><pre>
on hideDemo
  set cursor to watch
  <b>hide</b> titleBar
  lock screen
  <b>hide</b> bkgnd field "demo script"
  show bkgnd field "demo field"
  displayMessage "Let us go then you and I"
  unlock screen with dissolve
  wait 2 seconds
  lock screen
  <b>hide</b> bkgnd field "demo field"
  show bkgnd field "demo script"
  unlock screen with dissolve
  show titleBar
end hideDemo
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/bkgnd.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/window.md]

[embed:HelpExtras/Placeholders/externalWindow.md]

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [show](/HyperTalkReference/commands/show)
* [showPict](/HyperTalkReference/properties/showPict)
* [visible](/HyperTalkReference/properties/visible)
