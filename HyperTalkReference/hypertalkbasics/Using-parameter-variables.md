---
title: Using parameter variables
card_id: 10721
modified: yes
---

# Using parameter variables

A handler can receive values (called parameters) and use them as it runs. You represent each value with a <b>parameter variable</b>. A parameter variable always follows the handler name in a comma-separated list.

For example, when running the following `mouseUp` handler, HyperCard calls `sayMessage` with two values, `"red"` and `"apple"`. It then binds these values to the parameter variables `color` and `fruit` in the `sayMessage` handler.

```
on mouseUp
   sayMessage "red", "apple"
end mouseUp
on sayMessage color, fruit
   put "I want a" && color && fruit
end sayMessage
```

You can use the variables `color` and `fruit` anywhere inside the handler. When HyperCard sees them, it uses the values currently bound to them. (The variables remain bound only while the handler runs.)

## Demo Script

```
on mouseUp
  sayMessage "red", "apple"
end mouseUp

on sayMessage color, fruit
  put "I want a" && color && fruit & "." into the Message box
end sayMessage
```

## Related Topics

* [function](/HyperTalkReference/keywords/function)
* [on](/HyperTalkReference/keywords/on)
* [Writing function handlers](/HyperTalkReference/hypertalkbasics/Writing-function-handlers)
* [Writing message handlers](/HyperTalkReference/hypertalkbasics/Writing-message-handlers)
