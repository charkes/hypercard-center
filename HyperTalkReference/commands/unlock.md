---
title: unlock
card_id: 50046
---

# unlock

```
unlock {screen|messages|recent}
unlock error dialogs
unlock screen with [ph:effect] [[ph:speed]] ¬
        [to [ph:image]]
unlock screen with visual [effect] ¬
        [ph:effect] [[ph:speed]] [to [ph:image]]
```

`Unlock screen` lets HyperCard update the screen after a `lock screen` command. (Click the placeholders `[ph:effect]`, `[ph:speed]`, and `[ph:image]` to see their possible replacements.)

Optionally, you can add a single visual effect. You can lock the screen, perform actions on the card, and then unlock the screen with a visual effect.

`Unlock messages` lets `open`, `close`, `suspend`, and `resume` messages traverse the message-passing path.

`Unlock recent` lets HyperCard keep a visual record of visited cards in the Recent Cards dialog box.

`Unlock error dialogs` lets HyperCard show error dialog boxes when an error occurs.

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

```
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
```

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lock](/HyperTalkReference/commands/lock)
* [lockMessages](/HyperTalkReference/properties/lockMessages)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
