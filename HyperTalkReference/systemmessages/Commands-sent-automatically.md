---
title: Commands sent automatically
card_id: 3428
---

# Commands sent automatically

HyperCard sends some commands automatically in response to events, just as it sends system messages. But unlike system messages, if the command passes all the way to HyperCard, HyperCard performs a built-in action. So if you trap the command, the action won't happen.

HyperCard sends `choose` and `doMenu` as messages when the user chooses a tool or an item from one of HyperCard’s menus. It sends `close` as a message when the user clicks the close box of a window.

HyperCard sends `help` as a message when the user chooses Help from the Go menu (or presses Command-?).

HyperCard sends `arrowKey`, `commandKeyDown`, `controlKey`, `enterInField`, `enterKey`, `functionKey`, `keyDown`, `returnInField`, `returnKey`, and `tabKey` as messages when the user presses a key. It automatically sends `errorDialog` and `appleEvent` messages.

Click Related Topics for more information about each command.

## Related Topics

* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [arrowKey](/HyperTalkReference/commands/arrowKey)
* [choose](/HyperTalkReference/commands/choose)
* [close](/HyperTalkReference/commands/close)
* [commandKeyDown](/HyperTalkReference/commands/commandKeyDown)
* [controlKey](/HyperTalkReference/commands/controlKey)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [enterKey](/HyperTalkReference/commands/enterKey)
* [errorDialog](/HyperTalkReference/systemmessages/errorDialog)
* [functionKey](/HyperTalkReference/commands/functionKey)
* [help](/HyperTalkReference/commands/help)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [returnKey](/HyperTalkReference/commands/returnKey)
* [tabKey](/HyperTalkReference/commands/tabKey)
