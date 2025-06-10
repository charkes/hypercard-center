---
title: get
card_id: 38686
---

# get

<code><pre>
get [ph:expression]
get
</pre></code>

[<code>the
</pre></code>

]<code> [ph:property]
</pre></code>

[<code>of <i>object
</pre></code>

</i> ]

The <code>get</code> command puts the value of any expression or property into the local variable<code> it</code>.   

That is, 

   <code>get [ph:expression</code>]

is the same as 

   <code>put [ph:expression] into it</code> 


## Examples

```
get random(100) -- places a random number into the variable it
put it

get the short name of this card
if it is "Index" then ...

get the userLevel
if it < 3 then ...
```

## Demo Script

<code><pre>
<code><pre>
on getNumChars
 <b>get</b> the number of characters in bkgnd field "Demo Script"
 answer "This demo script contains" && it && "characters."
end getNumChars
</pre></code>
</pre></code>

## Related Topics

* [put](/HyperTalkReference/commands/put)
