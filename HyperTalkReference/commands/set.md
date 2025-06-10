---
title: set
card_id: 47503
---

# set

<code>set </code>[<code>the</code>]<code> [ph:property] to [ph:expression</code>] <code>set </code>[<code>the</code>]<code> [ph:property] of [ph:object] ¬     to [ph:expression</code>] <code><pre>

set
</pre></code>

[<code>the
</pre></code>

]<code> [ph:property] of [ph:window] ¬     to [ph:expression</code>] <code>set </code>[<code>the</code>] <code>property of</code> [[ph:<code>menuItem] of</code>]<code> ¬      [ph:menu] to [ph:expression] set </code>[<code>the</code>]<code> [ph:property] of [ph:chunk] ¬     of [ph:field] to [ph:expression</code>]

Note: <code>[ph:expression]</code> must yield a valid setting for the specified property. 

The <code>set</code> command changes the state of a specified property. If the object or element to which the property belongs is not specified, the property must be a global property or painting property. 

You can use the Info dialog box of an object to set many of its properties. 


## Examples

```
set the userLevel to 5
set the style of bkgnd button 1 to rectangle
set the wideMargins of card field id 34 to true
set the cantModify of this stack to true

set the top of Message box to (bottom of this card + 12)
set the scroll of card window to 0,0

set the enabled of menu 2 to false
set the cmdChar of first menuItem of second menu to "0"

set the textSize of field "Index" to (the textSize of field "Index" + 4)
set the textStyle of the clickChunk to bold
set the visible of menuBar to false
```

## Demo Script

<code><pre>
on madScroller
  put the rect of card window into theRect
  <b>set</b> the rect of card window to left of cd window,top of cd window,¬
  left of cd window + 172, top of cd window + 64
  repeat 10 times
    <b>set</b> the scroll of card window to ¬
    random(width of this card),random(height of this card)
    wait 30
  end repeat
  <b>set</b> the rect of card window to theRect
end madScroller
</pre></code>

## Related Topics

* [get](/HyperTalkReference/commands/get)
* [put](/HyperTalkReference/commands/put)
