---
title: lockRecent
card_id: 75404
---

# lockRecent

` set `[`the`]<code> lockRecent to [ph:trueOrFalse]

</code>The `lockRecent` property returns or sets whether HyperCard displays miniature pictures for the last 42 cards visited by the user (or a handler) in the Recent card dialog box. (`LockRecent `does not affect the trail of cards you can go back to.)

The default setting is false, meaning HyperCard <u>does</u> display miniature pictures of the cards visited. 

 Setting `lockRecent` to true speeds up scripts that go to cards.

HyperCard sets `lockRecent` to false on idle. 


## Examples

```
set the lockRecent to true
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lock](/HyperTalkReference/commands/lock)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
* [unlock](/HyperTalkReference/commands/unlock)
