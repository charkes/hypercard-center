---
title: filled
card_id: 71536
---

# filled

<code> set </code>[<code>the</code>]<code> filled to [ph:trueOrFalse] </code> The <code>filled</code> property returns or sets whether HyperCard fills shapes with the current pattern on the Patterns palette as you draw them. It corresponds to the Filled command in the Options menu (which appears when you select a Paint tool).

The default value is<code> false</code>. 

 The <code>filled</code> property affects the Rectangle, Rounded Rectangle, Oval, Curve, Regular Polygon, and Polygon tools. 


## Examples

```
set the filled to true
```

## Demo Script

<code><pre>
on mouseUp
  show bkgnd field "demo field"
  paintSetUp
  set <b>filled</b> to false
  choose rect tool
  displayMessage "Painting an UNFILLED shape:"
  drag from 180,100 to 300,220
  wait 2 seconds
  set <b>filled</b> to true
  choose oval tool
  displayMessage "Painting a FILLED shape:"
  drag from 180,100 to 300,220
  wait 1 second
  doMenu "Revert"
  hide bkgnd field "demo field"
  choose browse tool
end mouseUp

on paintSetUp
  show card pict
  set the dragSpeed to 125
  set the grid to false
  set the linesize to 2
  set the pattern to 33
  set the centered to false
end paintSetUp
</pre></code>

## Related Topics

* [centered](/HyperTalkReference/properties/centered)
* [multiple](/HyperTalkReference/properties/multiple)
* [multiSpace](/HyperTalkReference/properties/multiSpace)
* [reset](/HyperTalkReference/commands/reset)
