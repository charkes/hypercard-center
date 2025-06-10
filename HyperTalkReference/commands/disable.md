---
title: disable
card_id: 34993
---

# disable

<code><pre>
disable [ph:menu]
disable [ph:menuItem] of [ph:menu]
disable [ph:button]
</pre></code>

The <code>disable</code> command dims menu items, entire menus, and buttons. It’s a shortcut for setting the <code>enabled</code> property of a menu item,  menu, or button to <code>false</code>.  

Users cannot choose dimmed menu items.

Disabled buttons don't receive <code>mouseDown, mouseStillDown, mouseUp</code>, or <code>mouseDoubleClick</code> messages when you click them. 

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

<code><pre>
on disableTalkMenu
  if there is a menu "Reference" then
    <b>disable</b> menuItem "HyperTalk Reference" of menu "Reference"
  end if
end disableTalkMenu
</pre></code>

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
