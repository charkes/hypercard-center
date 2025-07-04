---
title: autoSelect
card_id: 12857
modified: yes
---

# autoSelect

```
set [the] autoSelect of [ph:field] ¬
     to [ph:trueOrFalse]
```

The `autoSelect` property sets or returns whether lines in a locked field highlight automatically in response to a `mouseDown` event and to dragging or shift-clicking.  (Such fields are called  <i>list fields</i>.)

The `autoSelect` property corresponds to the Auto Select check box in a Field Info dialog box.

Automatic highlighting occurs if `autoSelect`, `lockText`, and `dontWrap` are all set to `true`.

`AutoSelect` is set to false when `dontWrap` is set to false; `dontWrap` is set to true when `autoSelect` is set to true.

For `autoSelect` to affect more than one line in a locked field, that field's `multipleLines` property must also be set to `true`.

To learn which lines are selected, get the `selectedLine of [ph:field]`.  To learn the contents of those lines, get the `selectedText of [ph:field]`.  To preselect, use `select line x [to y] of [ph:field]`.

## Related Topics

* [dontWrap](/HyperTalkReference/properties/dontWrap)
* [lockText](/HyperTalkReference/properties/lockText)
* [multipleLines](/HyperTalkReference/properties/multipleLines)
* [select](/HyperTalkReference/commands/select)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
* [selectedText](/HyperTalkReference/functions/selectedText)
