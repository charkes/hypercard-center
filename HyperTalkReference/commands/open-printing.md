---
title: open printing
card_id: 42410
---

# open printing

<code>open printing </code>[<code>with dialog</code>]<code>

</code>The <code>open printing</code> command begins a print job. It uses the current settings from the Print Stack dialog box. 

If you specify the <code>with dialog o</code>ption, HyperCard displays the Print Stack dialog box, and the user can choose new settings. HyperCard sets<code> the result</code> to <code>Cancel</code> if the user clicks Cancel; otherwise, it sets <code>the result</code> to<code> empty</code>. 



You must use the <code>close printing</code> command to end a print job begun with<code> open printing.</code> 


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
