---
title: menuMessage
card_id: 76567
---

# menuMessage

`set [the] menuMessage of [ph:menuItem] of [ph:menu] to "[ph:messageName] [[ph:parameterList]]"`

The `menuMessage` property returns or sets the message sent to the current card when the user chooses a menu item from a menu.

The `menuMessage` property returns `empty` if the menu item has no associated message.

HyperCard’s default menu items have no associated messages sent to the current card unless they have been explicitly set with this property.

A `doMenu` handler can override a `menuMessage`.

## Examples

```
get the menuMessage of menuItem 1 of menu "Help"
if it is not empty then ...

set the menuMessage of menuItem "Print" of menu "File" to "myPrint"
set the menuMsg of menuItem 2 of menu 2 to "beep"
set the menuMsg of second menuItem of second menu to ¬
  "set the visible of field 1 to not the visible of field 1"
```

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [menus](/HyperTalkReference/functions/menus)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
