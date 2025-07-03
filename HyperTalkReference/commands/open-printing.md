---
title: open printing
card_id: 42410
---

# open printing

`open printing [with dialog]`

The `open printing` command begins a print job. It uses the current settings from the Print Stack dialog box.

If you specify the `with dialog` option, HyperCard displays the Print Stack dialog box, and the user can choose new settings. HyperCard sets `the result` to `Cancel` if the user clicks Cancel; otherwise, it sets `the result` to `empty`.

You must use the `close printing` command to end a print job begun with `open printing`.

## Examples

```
on printRange start,total
   -- print a range of cards from some start card
   push card  
   open printing  
   go to card start  
   print (total-start) + 1 cards  
   close printing  
   pop card  
end printRange
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [open report printing](/HyperTalkReference/commands/open-report-printing)
* [print](/HyperTalkReference/commands/print)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
* [reset](/HyperTalkReference/commands/reset)
