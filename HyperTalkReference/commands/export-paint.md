---
title: export paint
card_id: 36906
---

# export paint

<code>export paint to file [ph:fileName</code>]

The <code>export paint</code> command saves a Paint image of the current card to the specified file. <code>Export paint</code> works only when one of the Paint tools is chosen.

This command has the same effect as the Export Paint menu item that appears in the File menu (when a Paint tool is chosen), except that it avoids the dialog box that prompts the user for a file name. 

If <code>export paint</code> succeeds, HyperCard sets the function <code>the result</code> to <code>empty</code>; if the command fails (if, for example, you use<code> export paint</code> when the Browse tool is chosen), HyperCard sets <code>the result</code> to<code> "Couldn't export paint."</code> 


## Examples

```
export paint to file "Screen Dump 0"

ask file "Export paint to file:"
if it is not empty then export paint to file it
```

## Related Topics

* [import paint](/HyperTalkReference/commands/import-paint)
