---
title: start using
card_id: 48812
---

# start using

<code>start using [ph:stack</code>]

The <code>start using</code> command inserts the specified stack into the message-passing order between the current stack and the Home stack (or between the current stack and any other stacks being used).

Handlers in the stack script of the newly inserted stack can intercept messages as the messages move through the message-passing order. 

HyperCard records the full path name of the stacks being used as lines in the global property<code> the stacksInUse</code>. You can add up to 16 stacks.<code> </code> The first stack in use is on line 1 of <code>the stacksInUse</code>, the second stack is on line 2 of<code> the stacksInUse</code>, and so on. The order of items in<code> the StacksInUse</code> determines the message-passing order: from the current stack to line 1 of<code> the StacksInUse</code>, to line 2, and so on, to the Home stack. 


## Examples

```
start using stack "My Favorite Scripts"

answer file "What stack do you want to use?"
if it is not empty then start using stack it
```

## Related Topics

* [stacksInUse](/HyperTalkReference/properties/stacksInUse)
* [stop using](/HyperTalkReference/commands/stop-using)
