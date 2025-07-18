---
title: editBkgnd
card_id: 71150
---

# editBkgnd

`set [the] editBkgnd to [ph:trueOrFalse]`

The `editBkgnd` property returns or sets the layer where new painting or new buttons and fields will appear––in the card layer or in the background layer. It corresponds to the Background command in the Edit menu, and it’s available only when the user level is Painting (3) or higher.

The default setting is `false`, meaning that new images and  parts will appear on the card layer. 

## Examples

```
set the editBkgnd to true
```

## Demo Script

```
on mouseUp
  set cursor to watch
  set <b>editBkgnd</b> to true
  wait 2 seconds
  set <b>editBkgnd</b> to false
end mouseUp
```
