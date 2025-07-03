---
title: selectedField
card_id: 63565
---

# selectedField

```
the selectedField
```

Value returned: a field expression that indicates the field in which a range of characters is currently highlighted. If nothing is highlighted, it returns `empty`. The field expression returned has one of the following forms:

```
card field [ph:n]
bkgnd field [ph:n]
```

where `[ph:n]` is the number of the field.

## Examples

```
get the selectedField

put the selectedField into theField
```

## Demo Script

```
on selectedFieldDemo
  select line 1 of field 1
  wait 15
  answer "The field containing the selection is:" & return &¬
  the name of the selectedField
end selectedFieldDemo
```

## Related Topics

* [foundField](/HyperTalkReference/functions/foundField)
* [select](/HyperTalkReference/commands/select)
