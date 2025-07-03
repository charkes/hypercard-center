---
title: commandKeyDown
card_id: 8287
---

# commandKeyDown

```
commandKeyDown [ph:char]
```

The `commandKeyDown` command provides a way of sending a Command-key event from a handler. It acts exactly as if you had pressed Command at the same time as the specified character.

HyperCard sends the `commandKeyDown` command to a field (if the insertion point is set) or to the current card when the user presses a Command-key combination. The value passed to the parameter variable `[ph:char]` corresponds to the key pressed.

You can handle the `commandKeyDown` message as follows:

```
on commandKeyDown theKey
  [ph:statements]
end commandKeyDown
```

Note: `commandKeyDown` is not sent for characters typed using the `type` command.

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
