---
title: lockScreen
card_id: 75546
---

# lockScreen

`set [the] lockScreen to [ph:trueOrFalse]`

The `lockScreen` property returns or sets whether HyperCard updates the screen when you go to another card. You can use `lockScreen` to prevent the user from seeing cards as a handler goes to them.

The default setting is false. HyperCard sets `lockScreen` to false on idle.

Setting `lockScreen` to true speeds up scripts that go to cards momentarily before returning to the source card. (HyperCard runs faster when it doesn't have to redraw the screen.) 

## Examples

```
set the lockScreen to true
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lock](/HyperTalkReference/commands/lock)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [unlock](/HyperTalkReference/commands/unlock)
