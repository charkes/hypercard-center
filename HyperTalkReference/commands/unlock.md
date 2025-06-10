---
title: unlock
card_id: 50046
---

# unlock

<code><pre>
unlock {screen|messages|recent}
unlock error dialogs
unlock screen with [ph:effect]
</pre></code>

[<i><code>speed
</pre></code>

</i> ]<code> ¬        </code>[<code>to [ph:image</code>] ]<code> unlock screen with visual [effect] ¬        [ph:effect] </code>[[ph:<code>speed</code>] ]<code> </code>[<code>to [ph:image</code>] ]<code>

Unlock screen </code>lets HyperCard update the screen after a <code>lock screen</code> command. (Click the placeholders <code>[ph:effect], [ph:speed],</code> and<code> [ph:image]</code> to see their possible replacements.)

Optionally, you can add a single visual effect. You can lock the screen, perform 

actions on the card, and then unlock the screen with a visual effect.

<code>Unlock messages </code>lets <code>open, close, suspend,</code> and <code>resume</code> messages traverse the message-passing path.

<code>Unlock recent </code>lets HyperCard keep  a visual record of visited cards in the Recent Cards dialog box.

<code>Unlock error dialogs </code>lets HyperCard show error dialog boxes when an error occurs. 


## Examples

```
lock screen   -- same as "set lockScreen to TRUE"
unlock screen -- same as "set lockScreen to FALSE"

-- Use a visual effect, speed, and image:
unlock screen with dissolve slowly to inverse
unlock screen with visual effect dissolve
unlock screen with visual dissolve
unlock screen with dissolve

-- Use a variable to hold a visual effect:
put "visual effect dissolve" into effectVariable
unlock screen with effectVariable

unlock recent
unlock messages
```

## Demo Script

<code><pre>
on lockUnlockDemo
   -- Show and hide this field with visual effects:
   set cursor to watch
   lock screen
   hide field "Demo Script"
   unlock screen with shrink to center
   wait 1 second
   lock screen
   show field "Demo Script"
   unlock screen with stretch from center
end lockUnlockDemo
</pre></code>

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lock](/HyperTalkReference/commands/lock)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
