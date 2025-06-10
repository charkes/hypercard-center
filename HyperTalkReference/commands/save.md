---
title: save
card_id: 46772
---

# save

<code><pre>
save [this] stack as [stack] [ph:fileName]
save stack [ph:fileName] ¬
     as [stack] [ph:fileName]
</pre></code>

The <code>save</code> command saves a copy of a stack. It’s the same as choosing Save A Copy from the File menu, but it doesn't display a directory dialog box. Use <code>save</code> when you don't want a dialog box to interrupt a handler.

The form <code>save [this] stack</code> saves a copy of the current stack.

If the specified stack already exists, HyperCard sets the value of <code>the result</code> to <code>"Couldn’t duplicate stack."</code> You can test whether HyperCard saved the stack successfully as follows:

<code><pre>
save this stack as "My Copy"
if the result is not empty then ...
</pre></code>

## Examples

```
save this stack as stack "My Copy"

save stack as stack "Copy of" && the short name of this stack

save stack "Home" as stack "Copy of Home"
if the result is not empty then ...
```

## Related Topics

* [result](/HyperTalkReference/functions/result)
