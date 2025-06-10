---
title: import paint
card_id: 40224
---

# import paint

<code>import paint from file [ph:fileName]</code>

The <code>import paint</code> command loads a Paint image to the current card from a file. <code>Import paint</code> only works when one of the Paint tools is chosen.

This command has the same effect as the Import Paint menu item that appears in the File menu (when a Paint tool is chosen), except that it avoids the dialog box that prompts the user for a file name.

If <code>import paint</code> succeeds, HyperCard sets the function <code>the result</code> to <code>empty</code>; if the command fails (if, for example, you use<code> import paint</code> when the Browse tool is chosen), HyperCard sets <code>the result</code> to <code>"Couldn't import paint."</code>

## Examples

```
import paint from file "Sue’s Screen Dump"

answer file "Import paint from what file:" of type paint
if it is not empty then import paint from file it
```

## Related Topics

* [export paint](/HyperTalkReference/commands/export-paint)
