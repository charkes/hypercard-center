---
title: stacksInUse
card_id: 85008
modified: yes
---

# stacksInUse

`the stacksInUse`

The `stacksInUse` property returns a return-separated list of stacks that have been inserted into the message-passing path via the `start using` command.  Each stack appears in the order it will receive messages. The `stacksInUse` contains the full path names of the stacks being used.

HyperCard can use up to 16 stacks.

Note: You can’t compact a stack that’s being used.

## Examples

```
the number of lines of the stacksInUse -- total stacks in use
if "My Cool Scripts" is not in the stacksInUse then ... -- complain
```

## Demo Script

```
on whatStacksInUse
  answer "The stacks in use are:" & return & return & the stacksInUse
end whatStacksInUse
```

## Related Topics

* [start using](/HyperTalkReference/commands/start-using)
* [stop using](/HyperTalkReference/commands/stop-using)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
