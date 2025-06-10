---
title: multiSpace
card_id: 77376
---

# multiSpace

<code> set </code>[<code>the</code>]<code> multiSpace to [ph:posInteger]<u>

</code></u>where <code>[ph:posInteger]</code> is a number from 1 to 100.<code>

</code>The <code>multiSpace</code> property returns or sets the minimum amount of space, in pixels, between the edges of multiple shapes drawn when the <code>multiple</code> property is true. 

 The <code>multiSpace</code> property affects the Line, Rectangle, Rounded Rectangle, Oval, and Regular Polygon tools. Its default value is 1. 


## Examples

```
set the multiSpace to 10
```

## Demo Script

<code><pre>
<code><pre>
on multipleDemo
 show bkgnd field "Demo Field"
 setUpPaint
 displayMessage "      MultiSpace 2" & spaces(8) & "MultiSpace 5" & ¬
 spaces(9) & "MultiSpace 9"
 set the <b>multiSpace</b> to 2
 drawShape "100,160","160,220"
 set the <b>multiSpace</b> to 5
 drawShape "240,160","300,220"
 set the <b>multiSpace</b> to 9
 drawShape "380,160","440,220"
 wait 2 seconds
 domenu "revert"
 choose browse tool
 hide bkgnd field "Demo Field"
end multipleDemo
on drawShape  startTopLeft, endBotRight
 drag from startTopLeft to endBotRight with shiftKey
end drawShape
on setUpPaint
 choose oval tool
 set multiple to true
 set centered to true
 set dragspeed to 150
 set lineSize to 1
 set filled to false
 set grid to false
end setUpPaint
</pre></code>
</pre></code>

## Related Topics

* [centered](/HyperTalkReference/properties/centered)
* [filled](/HyperTalkReference/properties/filled)
* [multiple](/HyperTalkReference/properties/multiple)
