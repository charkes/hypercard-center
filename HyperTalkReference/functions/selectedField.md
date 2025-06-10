---
title: selectedField
card_id: 63565
---

# selectedField

<code><pre>
the selectedField
</pre></code>

Value returned: a field expression that indicates the field in which a range of characters is currently highlighted. If nothing is highlighted, it returns<code> empty</code>. The field expression returned has one of the following forms:

<code><pre>
card field [ph:n]
bkgnd field [ph:n]
</pre></code>

where <code>[ph:n]</code> is the number of the field. 


## Examples

```
get the selectedField

put the selectedField into theField
```

## Demo Script

<code><pre>
on selectedFieldDemo
  select line 1 of field 1
  wait 15
  answer "The field containing the selection is:" & return &¬
  the name of the selectedField
end selectedFieldDemo
</pre></code>

## Related Topics

* [foundField](/HyperTalkReference/functions/foundField)
* [select](/HyperTalkReference/commands/select)
