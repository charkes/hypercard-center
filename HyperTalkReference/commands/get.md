---
title: get
card_id: 38686
---

# get

```
get [ph:expression]
get [the] [ph:property] [of [ph:object]
```

The `get` command puts the value of any expression or property into the local variable `it`.   

That is, `get [ph:expression]` is the same as `put [ph:expression] into it`

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

```
on getNumChars
 <b>get</b> the number of characters in bkgnd field "Demo Script"
 answer "This demo script contains" && it && "characters."
end getNumChars
```

## Related Topics

* [put](/HyperTalkReference/commands/put)
