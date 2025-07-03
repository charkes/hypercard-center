---
title: import paint
card_id: 40224
---

# import paint

`import paint from file [ph:fileName]`

The `import paint` command loads a Paint image to the current card from a file. `Import paint` only works when one of the Paint tools is chosen.

This command has the same effect as the Import Paint menu item that appears in the File menu (when a Paint tool is chosen), except that it avoids the dialog box that prompts the user for a file name.

If `import paint` succeeds, HyperCard sets the function `the result` to `empty`; if the command fails (if, for example, you use` import paint` when the Browse tool is chosen), HyperCard sets `the result` to `"Couldn't import paint."`

## Examples

```
import paint from file "Sue’s Screen Dump"

answer file "Import paint from what file:" of type paint
if it is not empty then import paint from file it
```

## Related Topics

* [export paint](/HyperTalkReference/commands/export-paint)
