---
title: centered
card_id: 69837
---

# centered

`set [the] centered to [ph:trueOrFalse]`

The `centered` property returns or sets whether HyperCard draws shapes from the center rather than from a corner. It corresponds to the Centered command in the Options menu (which appears when you select a Paint tool).

The `centered` property affects the Line, Rectangle, Rounded Rectangle, and Oval tools. Its default value is `false`. 

## Examples

```
set the centered to true
```

## Demo Script

```
on mouseUp
  show bkgnd field "demo field"
  setUpPaint  -- See Below
  displayMessage "Drag with centered set to TRUE:"
  set the <b>centered</b> to true
  drag from 240,160 to 305,225 with optionKey
  wait 2 seconds
  displayMessage "The same drag with centered set to FALSE:"
  set the <b>centered</b> to false
  drag from 240,160 to 305,225
  wait 2 seconds
  doMenu "Revert"
  put empty into bkgnd field "demo field"
  hide bkgnd field "demo field"
  choose browse tool
end mouseUp

on setUpPaint
  choose rect tool
  set pattern to 22
  set the linesize to 2
  set filled to false
  set the dragSpeed to 100
  set multiSpace to 4
  set multiple to true
end setUpPaint
```

## Related Topics

* [filled](/HyperTalkReference/properties/filled)
* [multiple](/HyperTalkReference/properties/multiple)
* [multiSpace](/HyperTalkReference/properties/multiSpace)
* [reset](/HyperTalkReference/commands/reset)
