---
title: dontWrap
card_id: 84490
---

# dontWrap

```
set [the] dontWrap of [ph:field] ¬
     to [ph:trueOrFalse]
```

The `dontWrap` property returns or sets whether a field wraps text that is longer than the width of the field or instead truncates the viewable text at the right edge of the field. (In HyperTalk, a return character determines a line.)

This property corresponds to the Don’t Wrap option in a Field Info dialog box.

Truncated viewable text isn't lost. If you set the `dontWrap` to `true`, the “missing” text appears in the field.

This property is set to true when `autoSelect` is set to true; and it sets `autoSelect` to false when it is set to false.

## Examples

```
set the dontWrap of card field "Index" of last card to false
```

## Demo Script

```
on toggleWrap
 set the cursor to watch
 set the <b>dontWrap</b> of me to true
 wait 2 sec
 set the <b>dontWrap</b> of me to false
end toggleWrap
-- Here is some text that will illustrate the dontWrap feature:
-- Normally, when dontWrap is set to false, the text wraps to the next display line of the field.
-- When dontWrap is set to true, the text does not wrap to the next line; the field looks more like a list.
```

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
