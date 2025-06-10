---
title: copy template
card_id: 95696
---

# copy template

<code><pre>
copy template [ph:templateName] ¬
               to [ph:stack]
</pre></code>

The <code>copy template</code> command makes a copy of printing report template <code>[ph:templateName]</code> from the current stack and moves it into the stack <code>[ph:stack]</code>.

## Examples

```
copy template "Monthly Report" to stack "Business Plan"

copy template theTemplate to stack theStack
```

## Related Topics

* [reportTemplates](/HyperTalkReference/properties/reportTemplates)
