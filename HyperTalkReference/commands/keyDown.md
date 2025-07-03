---
title: keyDown
card_id: 40449
---

# keyDown

`keyDown [ph:char]`

The `keyDown` command simulates a key press from within a handler. It acts exactly as if the user pressed a character` `from the keyboard.

HyperCard sends the `keyDown` command to a field (if the insertion point is set) or to the current card when the user presses a key. The value passed to the parameter variable `[ph:char]` corresponds to the key pressed.

You can handle the `keyDown` message as follows:

```
on keyDown theKey
  [ph:statements]
end keyDown
```

Note: `keyDown` is not sent for characters typed using the `type` command.

## Demo Script

```
on keyDownDemo
  -- The <b>keyDown</b> messages are handled in the script of this card
  show bkgnd field "demo field"
  put "Type any key..." into bkgnd field "demo field"
  put "Press the Return key to continue..." into ¬
  line 6 of bkgnd field "demo field"
end keyDownDemo
```

## Related Topics

* [commandKeyDown](/HyperTalkReference/commands/commandKeyDown)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [controlKey](/HyperTalkReference/commands/controlKey)
* [optionKey](/HyperTalkReference/functions/optionKey)
* [shiftKey](/HyperTalkReference/functions/shiftKey)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
