---
title: disable
card_id: 34993
---

# disable

```
disable [ph:menu]
disable [ph:menuItem] of [ph:menu]
disable [ph:button]
```

The `disable` command dims menu items, entire menus, and buttons. It’s a shortcut for setting the `enabled` property of a menu item,  menu, or button to `false`.  

Users cannot choose dimmed menu items.

Disabled buttons don't receive `mouseDown, mouseStillDown, mouseUp`, or `mouseDoubleClick` messages when you click them.

## Examples

```
disable menu "File"
disable menu 2
disable second menu

disable menuItem "New" of menu "File"
disable menuItem 2 of menu 2
disable second menuItem of second menu

disable button 1
disable background button id 1234
```

## Demo Script

```
on disableTalkMenu
  if there is a menu "Reference" then
    <b>disable</b> menuItem "HyperTalk Reference" of menu "Reference"
  end if
end disableTalkMenu
```

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menus](/HyperTalkReference/functions/menus)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
