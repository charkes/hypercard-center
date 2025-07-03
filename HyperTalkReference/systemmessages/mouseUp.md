---
title: mouseUp
card_id: 21197
---

# mouseUp

```
mouseUp
```

Handler:

```
on mouseUp
  [ph:statements]
end mouseUp
```

HyperCard sends the `mouseUp` message to a button or locked field when the user releases the mouse button[ph:and]  the pointer is inside the rectangle of the same button or field it was in when the user pressed the mouse button.

HyperCard sends `mouseUp` to the current card when the user both presses [ph:and ]releases the mouse button while the pointer is not in the rectangle of a button or field.

## Demo Script

```
on <b>mouseUp</b>
  answer "Hello"
end <b>mouseUp</b>
```

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouse](/HyperTalkReference/functions/mouse)
* [mouseClick](/HyperTalkReference/functions/mouseClick)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
