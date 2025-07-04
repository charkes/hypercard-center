---
title: open report printing
card_id: 42512
---

# open report printing

```
open report printing
open report printing with dialog
open report printing ¬
    with template [ph:text]
```

where `[ph:text]` is the name of a report template in the current stack.

The `open report printing` command begins the process of printing a stack (or part of a stack) as a report. It uses the current settings from the Print Report dialog box. You must use the `close printing` command to end a job begun with `open report printing`.

If you specify the `with dialog` option, HyperCard displays the Print Report dialog box and the user can choose new settings. If you specify the `with template` option, HyperCard prints the stack with the named report template.

HyperCard sets the function `the result` to `Cancel` if the user clicks Cancel in the dialog box, to `no such report template` if you specify a template that doesn’t exist, or to `empty` in all other cases.

## Examples

```
-- An example script for printing mailing labels, assuming a
-- report template Mailing Labels already exists:

on printLabels
  open report printing with template "Mailing Labels" -- choose template
  print all cards -- specify what cards to print
  close printing -- generate the report and print it
end printLabels
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [open printing](/HyperTalkReference/commands/open-printing)
* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
* [reportTemplates](/HyperTalkReference/properties/reportTemplates)
* [reset](/HyperTalkReference/commands/reset)
