---
title: foundField
card_id: 56310
---

# foundField

```
the foundField
```

Value returned: a field expression that identifies the field in which the most recent `find` command located its target string. If nothing was found, it returns `empty`. The field expression returned has one of the following forms:

```
card field [ph:n]
bkgnd field [ph:n]
```

where `[ph:n]` is the number of the field.


## Examples

```
find "Kathy"
put the foundField
```

## Demo Script

```
on foundFieldDemo
   find "foundFieldDemo"
   answer "The foundField is" && the <b>foundField</b>  & "." & ¬
   return & return &¬
   "The name of the foundField is" && the name of the <b>foundField</b> &¬
   "."
end foundFieldDemo
```

## Related Topics

* [find](/HyperTalkReference/commands/find)
* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [selectedField](/HyperTalkReference/functions/selectedField)
