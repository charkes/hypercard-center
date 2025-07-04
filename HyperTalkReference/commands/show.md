---
title: show
card_id: 47827
modified: yes
---

# show

```
show menuBar
show titleBar
show groups
show all cards
show marked cards

show [ph:posInteger] cards
show card picture
show background picture
show picture of [ph:card]
show picture of [ph:bkgnd]

show [ph:field] [at [ph:point]]
show [ph:button] [at [ph:point]]

show [ph:window] [at [ph:point]]
show [ph:externalWindow] [at [ph:point]]
```

The `show` command displays HyperCard objects and elements.

`Show menuBar` displays the menu bar at the top of the screen (unless the screen is locked). `Show titleBar` displays the title bar on the card window if it’s been hidden. (Normally, the title bar is visible.)

`Show groups` displays a two-pixel gray underline for all text that has the `group` text style. (By default, the `group` text style is invisible.) The underline appears for grouped text in every field (in all stacks). Use the `hide groups` command to remove the underline.

The `show card` forms display the specified cards in the current stack in turn, beginning with the next card or the next marked card.

The other forms of the `show` command display the card or background picture, a window, or an object at a specified location on the screen. If the point is not given, the window or object is displayed at its previous location.

Showing a window makes it the frontmost window. With external windows, an external command or external function must first create a window before `show` will work on it. `Show` does <b>not</b> create windows.

## Examples

```
-- show a series of cards
show all cards  
show ten cards  

put 26 into howMany  
show howMany cards

show card window

-- built-in windows:
show tool window
show window "tools"
show Message box at 100,100
show window "Message"
show message watcher
show window "Message Watcher"
show variable watcher
show window "Variable Watcher" at 70,280

-- external windows:
show window (line 9 of the windows)
show window "Navigator" -- only if it already exists
show window "Script of My HD:Home" at 100,100 -- only if it is open

-- show objects:
show card field 1
show field "Names" at 1,1  
show bkgnd btn id 35 at 10,10

-- show the picture of a specified card or bkgnd:

show picture of card 3
show pict of first cd
show picture of background "jazz"
```

## Demo Script

```
on showPictureDemo
  -- draw a picture and show it only when done:
  <b>show</b> bkgnd field "demo field"
  hide card picture
  drawPicture -- see below
  <b>show card picture
</b>  displayMessage "Click the mouse" & return & "to continue..."
  set the cursor to arrow
  wait until the mouseClick
  lock screen
  doMenu "revert" -- Don't keep the new picture
  choose browse tool
  unlock screen with dissolve slowly
  hide bkgnd field "demo field"
end showPictureDemo

on drawPicture
  setUpPaint
  put "50,16,12,10,9,8,7,6,5,4,3" into theSides
  repeat with itemNum = 1 to the number of items in theSides
    set polysides to (item itemNum of theSides)
    drag from "240,160" to "240,250"
  end repeat
end drawPicture

on setUpPaint
  set lineSize to 1
  choose regular polygon tool
  set the pattern to 1
  set centered to true
  set filled to true
  set grid to false
end setUpPaint
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [hide](/HyperTalkReference/commands/hide)
* [location](/HyperTalkReference/properties/location)
* [mark](/HyperTalkReference/commands/mark)
* [showPict](/HyperTalkReference/properties/showPict)
* [visible](/HyperTalkReference/properties/visible)
* [visual](/HyperTalkReference/commands/visual)
