---
title: pass
card_id: 27256
modified: yes
---

# pass

```
pass [ph:functionName]
pass [ph:messageName]
```

The `pass` keyword ends execution of the current handler and sends the entire message that initiated execution of the handler to the next object in the message-passing order.

(Ordinarily, once a message is handled, it does <i>not</i> continue along the message- passing order.)

In general, a stack should pass any system messages that it handles so that other stacks later in the message-passing order also get a chance to handle the message.

For example, a `mouseWithin` handler in your Home stack won't ever run if you also have a `mouseWithin` handler without a `pass` statement in a stack before Home in the message-passing path.

## Examples

```
on openCard
  put the number of this card
  pass openCard -- so other openCard handlers can run
end openCard
```

## Related Topics

* [Handling messages](/HyperTalkReference/hypertalkbasics/Handling-messages)
* [on](/HyperTalkReference/keywords/on)
* [send](/HyperTalkReference/keywords/send)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
