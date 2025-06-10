---
title: multiple
card_id: 77229
---

# multiple

<code> set </code>[<code>the</code>]<code> multiple to [ph:trueOrFalse]

</code>The <code>multiple</code> property returns or sets whether HyperCard draws multiple images when the user (or a handler) drags with a Paint tool. It corresponds to the Draw Multiple command in the Options menu (which appears when you select a Paint tool).  

The <code>multiSpace</code> property affects the number of multiple shapes drawn. 

 The <code>multiple</code> property affects the Line, Rectangle, Rounded Rectangle, Oval, and Regular Polygon tools. Its default value is false. 


## Examples

```
set the multiple to true
```

## Demo Script

<code><pre>
<code><pre>
on multipleDemo
 setUpPaint
 set <b>multiple</b> to false
 set dragspeed to 150
 drag from "240,150" to "290,230"
 set <b>multiple</b> to true
 drag from "240,150" to "290,230"
 wait 25
 domenu "revert"
 choose browse tool
end multipleDemo
on setUpPaint
 set lineSize to 2
 choose regular polygon tool
 set polysides to 4
 show card picture
 set centered to true
 set filled to false
 set grid to false
 set multiSpace to 5
end setUpPaint
</pre></code>
</pre></code>

## Related Topics

* [centered](/HyperTalkReference/properties/centered)
* [filled](/HyperTalkReference/properties/filled)
* [multiSpace](/HyperTalkReference/properties/multiSpace)
* [reset](/HyperTalkReference/commands/reset)
