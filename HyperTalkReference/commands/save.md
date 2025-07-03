---
title: save
card_id: 46772
---

# save

```
save [this] stack as [stack] [ph:fileName]
save stack [ph:fileName] ¬
     as [stack] [ph:fileName]
```

The `save` command saves a copy of a stack. It’s the same as choosing Save A Copy from the File menu, but it doesn't display a directory dialog box. Use `save` when you don't want a dialog box to interrupt a handler.

The form `save [this] stack` saves a copy of the current stack.

If the specified stack already exists, HyperCard sets the value of `the result` to `"Couldn’t duplicate stack."` You can test whether HyperCard saved the stack successfully as follows:

```
save this stack as "My Copy"
if the result is not empty then ...
```

## Examples

```
save this stack as stack "My Copy"

save stack as stack "Copy of" && the short name of this stack

save stack "Home" as stack "Copy of Home"
if the result is not empty then ...
```

## Related Topics

* [result](/HyperTalkReference/functions/result)
