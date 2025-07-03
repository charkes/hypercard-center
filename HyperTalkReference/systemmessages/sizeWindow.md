---
title: sizeWindow
card_id: 16789
---

# sizeWindow

```
sizeWindow
```

Handler:

```
on sizeWindow
  [ph:statements]
end sizeWindow
```

HyperCard sends the `sizeWindow` message to the current card when the user or a script resizes the window. In many cases, HyperCard will send a `moveWindow` message immediately after  a `sizeWindow` message.

Here are the ways a window can be resized:

* The user resizes the window using the size box.
* The user resizes the window using the Scroll window.
* The user clicks the zoom box, and the zoom changes the window size.
* A handler sets the `rect` of the card window to a new size.
* A handler resizes all the cards in a stack by setting the `rect` of the card to a new size. 

## Related Topics

* [moveWindow](/HyperTalkReference/systemmessages/moveWindow)
* [close](/HyperTalkReference/commands/close)
