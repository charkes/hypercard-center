---
title: showLines
card_id: 82338
---

# showLines

`set [the] showLines of [ph:field] to [ph:trueOrFalse]`

The `showLines` property returns or sets whether the text baselines of a field appear. It corresponds to the Show Lines check box in a Field Info dialog box.

The default value is false (meaning that the baselines are invisible).

Setting the `showLines` property to true sets the `fixedLineHeight `property to true. Setting `the showLines` to false has no effect on `the fixedLineHeight`.

Note: The `showLines` property  has no effect for scrolling fields.

## Examples

```
set the showLines of bkgnd field "First Name" to true
```

## Demo Script

```
on showMyLines
 set <b>showLines </b>of bkgnd field "demo script" to "true"
 set the style of bkgnd field "demo script" to rect -- to show lines
 wait 2 seconds
 set the style of bkgnd field "demo script" to scrolling
 set <b>showLines </b>of bkgnd field "demo script" to "false"
end showMyLines
```

## Related Topics

* [fixedLineHeight](/HyperTalkReference/properties/fixedLineHeight)
