---
title: cantAbort
card_id: 68357
---

# cantAbort

` set `[`the`] <code>cantAbort of [ph:stack] ¬     to [ph:trueOrFalse]

</code>The `cantAbort` property returns or sets whether users can type Command-. (Command-period) to stop any running handlers. It corresponds to the Can’t Abort check box in the Protect Stack dialog box. Use `cantAbort` to prevent users from canceling certain critical operations that would leave a stack in a confusing or dangerous state. 

<b> Warning</b>: Use `cantAbort` with caution.  Once `cantAbort` is set to true, there's no way to halt an errant handler.  Set ` cantAbort `to true, and then immediately set it to false when you no longer need it. 


## Examples

```
set the cantAbort of this stack to true
set the cantAbort of this stack to false
```

