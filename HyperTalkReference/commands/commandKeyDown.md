---
title: commandKeyDown
card_id: 8287
---

# commandKeyDown

<code><pre>
commandKeyDown [ph:char]
</pre></code>

The <code>commandKeyDown</code> command provides a way of sending a Command-key event from a handler. It acts exactly as if you had pressed Command at the same time as the specified character.

HyperCard sends the <code>commandKeyDown</code> command to a field (if the insertion point is set) or to the current card when the user presses a Command-key combination. The value passed to the parameter variable <code>[ph:char]</code> corresponds to the key pressed. 

You can handle the <code>commandKeyDown</code> message as follows:

<code><pre>
on commandKeyDown theKey
  [ph:statements]
end commandKeyDown
</pre></code>

Note: <code>commandKeyDown</code> is not sent for characters typed using the <code>type</code> command. 


## Examples

```
commandKeyDown "V" -- paste; same as type "v" with commandKey
commandKeyDown "B" -- edit background

on commandKeyDown theKey
  if theKey = "?" then goMyHelp -- trap normal help key
  else pass commandKeyDown
end commandKeyDown
```

## Related Topics

* [commandKey](/HyperTalkReference/functions/commandKey)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
