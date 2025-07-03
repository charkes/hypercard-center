---
title: lock
card_id: 40922
---

# lock

```
lock {messages|recent|screen}
lock error dialogs
```

`Lock messages` has the same effect as `set lockMessages to true`: it prevents HyperCard from sending `open`, `close` `suspend`, and `resume` system messages along the message-passing path.

`Lock recent` has the same effect as `set lockRecent to true`: it prevents HyperCard from keeping a visual record of cards visited by the user (or a handler) in the Recent Card dialog box.

`Lock screen` has the same effect as setting the property `lockScreen` to `true`: it prevents HyperCard from updating the screen.

`Lock error dialogs` prevents error dialog boxes from appearing; instead, the message `errorDialog [ph:errorMessage]` is sent to the current card.

Locking is automatically unlocked at idle time.

## Demo Script

```
on mouseUp
  -- with the screen not locked:
  hide bkgnd button "Run the Script"
  wait 20
  hide bkgnd button "Close"
  wait 20
  hide bkgnd button id 57
  wait 20
  hide bkgnd field "Demo Script"
  wait 20
  hide bkgnd button "Panel"
  wait 30
  --with the screen locked:
  <b>lock screen</b>
  show bkgnd button "Panel"
  show bkgnd field "Demo Script"
  show bkgnd button id 57
  show bkgnd button "Close"
  show bkgnd button "Run the Script"
  unlock screen with checkerboard
end mouseUp
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
* [unlock](/HyperTalkReference/commands/unlock)
