---
title: Where messages are sent initially
card_id: 6031
---

# Where messages are sent initially

HyperCard automatically sends system messages and a few commands to one of three objects: a specific button, a specific field, or the current card. If none of these objects handles the message, it continues along the message-passing order until it reaches HyperCard itself.

The commands HyperCard sends automatically deal with keyboard events and menu events.

Click an object to see the messages it can receive from HyperCard.

### Buttons

The following system messages are initially sent to a specific button:

```
deleteButton
mouseDoubleClick
mouseDown
mouseEnter
mouseLeave
mouseStillDown
mouseUp
mouseWithin
newButton
```

### Fields

The following commands (in bold) and system messages are initially sent to a specific field:

```
closeField, commandKeyDown,
deleteField, enterInField,
exitField, keyDown,
mouseDoubleClick, mouseDown, mouseEnter,
mouseLeave, mouseStillDown,
mouseUp, mouseWithin,
newField, openField,
returnInField, tabKey
```

### The current card

The following commands (in bold) and system messages are initially sent to the current card:

```
appleEvent, arrowKey, choose, close, closeBackground, closeCard, closeStack, commandKeyDown, controlKey, deleteBackground, deleteCard, deleteStack, doMenu, enterKey, functionKey, help, hide, idle, keyDown, mouseDoubleClick, mouseDown, mouseStillDown, mouseUp, moveWindow, newBackground, newCard, newStack, openBackground, openCard, openStack, quit, resume, resumeStack, returnKey, show, sizeWindow, startUp, suspend, suspendStack, tabKey
```

## Related Topics

* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [arrowKey](/HyperTalkReference/commands/arrowKey)
* [choose](/HyperTalkReference/commands/choose)
* [close](/HyperTalkReference/commands/close)
* [closeBackground](/HyperTalkReference/systemmessages/closeBackground)
* [closeCard](/HyperTalkReference/systemmessages/closeCard)
* [closeField](/HyperTalkReference/systemmessages/closeField)
* [closeStack](/HyperTalkReference/systemmessages/closeStack)
* [commandKeyDown](/HyperTalkReference/commands/commandKeyDown)
* [controlKey](/HyperTalkReference/commands/controlKey)
* [deleteBackground](/HyperTalkReference/systemmessages/deleteBackground)
* [deleteButton](/HyperTalkReference/systemmessages/deleteButton)
* [deleteCard](/HyperTalkReference/systemmessages/deleteCard)
* [deleteField](/HyperTalkReference/systemmessages/deleteField)
* [deleteStack](/HyperTalkReference/systemmessages/deleteStack)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enterInField](/HyperTalkReference/commands/enterInField)
* [enterKey](/HyperTalkReference/commands/enterKey)
* [exitField](/HyperTalkReference/systemmessages/exitField)
* [functionKey](/HyperTalkReference/commands/functionKey)
* [help](/HyperTalkReference/commands/help)
* [hide](/HyperTalkReference/commands/hide)
* [idle](/HyperTalkReference/systemmessages/idle)
* [keyDown](/HyperTalkReference/commands/keyDown)
* [Message sending orders](/HyperTalkReference/systemmessages/Message-sending-orders)
* [mouseDown](/HyperTalkReference/systemmessages/mouseDown)
* [mouseEnter](/HyperTalkReference/systemmessages/mouseEnter)
* [mouseLeave](/HyperTalkReference/systemmessages/mouseLeave)
* [mouseStillDown](/HyperTalkReference/systemmessages/mouseStillDown)
* [mouseUp](/HyperTalkReference/systemmessages/mouseUp)
* [mouseWithin](/HyperTalkReference/systemmessages/mouseWithin)
* [moveWindow](/HyperTalkReference/systemmessages/moveWindow)
* [newBackground](/HyperTalkReference/systemmessages/newBackground)
* [newButton](/HyperTalkReference/systemmessages/newButton)
* [newCard](/HyperTalkReference/systemmessages/newCard)
* [newField](/HyperTalkReference/systemmessages/newField)
* [newStack](/HyperTalkReference/systemmessages/newStack)
* [openBackground](/HyperTalkReference/systemmessages/openBackground)
* [openCard](/HyperTalkReference/systemmessages/openCard)
* [openField](/HyperTalkReference/systemmessages/openField)
* [openStack](/HyperTalkReference/systemmessages/openStack)
* [quit](/HyperTalkReference/systemmessages/quit)
* [resume](/HyperTalkReference/systemmessages/resume)
* [resumeStack](/HyperTalkReference/systemmessages/resumeStack)
* [returnInField](/HyperTalkReference/commands/returnInField)
* [returnKey](/HyperTalkReference/commands/returnKey)
* [show](/HyperTalkReference/commands/show)
* [sizeWindow](/HyperTalkReference/systemmessages/sizeWindow)
* [startUp](/HyperTalkReference/systemmessages/startUp)
* [suspend](/HyperTalkReference/systemmessages/suspend)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
* [tabKey](/HyperTalkReference/commands/tabKey)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
