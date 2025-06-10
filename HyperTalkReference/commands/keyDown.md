---
title: keyDown
card_id: 40449
---

# keyDown

<code>keyDown [ph:char</code>]

The <code>keyDown</code> command simulates a key press from within a handler. It acts exactly as if the user pressed a character<code> </code>from the keyboard.

HyperCard sends the <code>keyDown</code> command to a field (if the insertion point is set) or to the current card when the user presses a key. The value passed to the parameter variable <code>[ph:char]</code> corresponds to the key pressed. 

You can handle the <code>keyDown</code> message as follows:

<code><pre>
on keyDown theKey
  [ph:statements]
end keyDown
</pre></code>

Note: <code>keyDown</code> is not sent for characters typed using the <code>type</code> command. 


## Demo Script

<code><pre>
on keyDownDemo
  -- The <b>keyDown</b> messages are handled in the script of this card
  show bkgnd field "demo field"
  put "Type any key..." into bkgnd field "demo field"
  put "Press the Return key to continue..." into ¬
  line 6 of bkgnd field "demo field"
end keyDownDemo
</pre></code>

## Related Topics

* [commandKeyDown](/HyperTalkReference/commands/commandKeyDown)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [controlKey](/HyperTalkReference/commands/controlKey)
* [optionKey](/HyperTalkReference/functions/optionKey)
* [shiftKey](/HyperTalkReference/functions/shiftKey)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
