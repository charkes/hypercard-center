---
title: showName
card_id: 82576
---

# showName

<code> set </code>[<code>the</code>]<code> showName of [ph:button] ¬     to [ph:trueOrFalse]

</code>The <code>showName</code> property returns or sets whether HyperCard displays the name of a button (if the button has one) within the button’s rectangle. It corresponds to the Show Name check box in a Button Info dialog box. 


## Examples

```
set the showName of bkgnd button "Index" to true
```

## Demo Script

<code><pre>
<code><pre>
on hideBtnName
 set <b>showName </b>of bkgnd button "Run the Script" to "false"
 wait 30
 set <b>showName </b>of bkgnd button "Run the Script" to "true"
end hideBtnName
</pre></code>
</pre></code>

## Related Topics

* [textAlign](/HyperTalkReference/properties/textAlign)
* [textFont](/HyperTalkReference/properties/textFont)
* [textStyle](/HyperTalkReference/properties/textStyle)
