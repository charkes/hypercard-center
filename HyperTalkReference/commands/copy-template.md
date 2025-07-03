---
title: copy template
card_id: 95696
---

# copy template

```
copy template [ph:templateName] ¬
               to [ph:stack]
```

The `copy template` command makes a copy of printing report template `[ph:templateName]` from the current stack and moves it into the stack `[ph:stack]`.

## Examples

```
copy template "Monthly Report" to stack "Business Plan"

copy template theTemplate to stack theStack
```

## Related Topics

* [reportTemplates](/HyperTalkReference/properties/reportTemplates)
