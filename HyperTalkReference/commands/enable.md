---
title: enable
card_id: 61996
---

# enable

```
enable [ph:menu]
enable [ph:menuItem] of [ph:menu]
enable [ph:button]
```

The `enable` command activates menu items, entire menus, or buttons that are  inactive (dimmed).  It’s a shortcut for setting the `enabled` property to `true`.

The `enable` command enables only items in HyperCard’s menus that are currently available to the user.  For example, the following command will not enable the Button Info command in the Objects menu unless a button is currently selected:

`enable menuItem 1 of menu "Objects"`

## Examples

```
enable menu "File"
enable menu 2
enable second menu

enable menuItem "New" of menu "File"
enable menuItem 2 of menu 2
enable second menuItem of second menu

enable background button 3
enable last button
```

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menus](/HyperTalkReference/functions/menus)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
