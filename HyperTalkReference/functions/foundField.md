---
title: foundField
card_id: 56310
---

# foundField

<code><pre>
the foundField
</pre></code>

Value returned: a field expression that identifies the field in which the most recent <code>find</code> command located its target string. If nothing was found, it returns<code> empty</code>. The field expression returned has one of the following forms:

<code><pre>
card field [ph:n]
bkgnd field [ph:n]
</pre></code>

where <code>[ph:n]</code> is the number of the field. 


## Examples

```
find "Kathy"
put the foundField
```

## Demo Script

<code><pre>
on foundFieldDemo
   find "foundFieldDemo"
   answer "The foundField is" && the <b>foundField</b>  & "." & ¬
   return & return &¬
   "The name of the foundField is" && the name of the <b>foundField</b> &¬
   "."
end foundFieldDemo
</pre></code>

## Related Topics

* [find](/HyperTalkReference/commands/find)
* [foundChunk](/HyperTalkReference/functions/foundChunk)
* [selectedField](/HyperTalkReference/functions/selectedField)
