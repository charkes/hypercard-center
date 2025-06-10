---
title: lock
card_id: 40922
---

# lock

<code><pre>
lock {messages|recent|screen}
lock error dialogs
</pre></code>

<code>Lock messages </code>has the same effect as <code>set lockMessages to true</code>: it prevents HyperCard from sending <code>open</code>, <code>close, suspend,</code> and <code>resume</code> system messages along the message-passing path.

<code>Lock recent </code>has the same effect as<code> set lockRecent to true</code>: it prevents HyperCard from keeping  a visual record of cards visited by the user (or a handler) in the Recent Card dialog box. 

<code>Lock screen</code> has the same effect as setting the property <code>lockScreen</code> to <code>true</code>: it prevents HyperCard from updating the screen.

<code>Lock error dialogs </code>prevents error dialog boxes from appearing; instead, the message <code>errorDialog [ph:errorMessage]</code> is sent to the current card. <code>

</code>Locking is automatically unlocked at idle time. 


## Demo Script

<code><pre>
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
</pre></code>

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
* [unlock](/HyperTalkReference/commands/unlock)
