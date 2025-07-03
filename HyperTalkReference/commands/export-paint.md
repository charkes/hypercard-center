---
title: export paint
card_id: 36906
---

# export paint

`export paint to file [ph:fileName]`

The `export paint` command saves a Paint image of the current card to the specified file. `Export paint` works only when one of the Paint tools is chosen.

This command has the same effect as the Export Paint menu item that appears in the File menu (when a Paint tool is chosen), except that it avoids the dialog box that prompts the user for a file name.

If `export paint` succeeds, HyperCard sets the function `the result` to `empty`; if the command fails (if, for example, you use` export paint` when the Browse tool is chosen), HyperCard sets `the result` to `"Couldn't export paint."`

## Examples

```
export paint to file "Screen Dump 0"

ask file "Export paint to file:"
if it is not empty then export paint to file it
```

## Related Topics

* [import paint](/HyperTalkReference/commands/import-paint)
