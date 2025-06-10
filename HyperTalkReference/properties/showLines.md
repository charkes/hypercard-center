---
title: showLines
card_id: 82338
---

# showLines

<code> set </code>[<code>the</code>]<code> showLines of [ph:field] ¬     to [ph:trueOrFalse]

</code>The <code>showLines</code> property returns or sets whether the text baselines of a field appear. It corresponds to the Show Lines check box in a Field Info dialog box.

The default value is false (meaning that the baselines are invisible). 

 Setting the <code>showLines</code> property to true sets the <code>fixedLineHeight </code>property to true. Setting <code>the showLines</code> to false has no effect on<code> the fixedLineHeight</code>.

Note: The <code>showLines</code> property  has no effect for scrolling fields. 


## Examples

```
set the showLines of bkgnd field "First Name" to true
```

## Demo Script

<code><pre>
<code><pre>
on showMyLines
 set <b>showLines </b>of bkgnd field "demo script" to "true"
 set the style of bkgnd field "demo script" to rect -- to show lines
 wait 2 seconds
 set the style of bkgnd field "demo script" to scrolling
 set <b>showLines </b>of bkgnd field "demo script" to "false"
end showMyLines
</pre></code>
</pre></code>

## Related Topics

* [fixedLineHeight](/HyperTalkReference/properties/fixedLineHeight)
