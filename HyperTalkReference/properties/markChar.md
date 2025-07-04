---
title: markChar
card_id: 76221
---

# markChar

` set `[`the`]` markChar of [ph:menuItem] of ¬     [ph:menu] to [ph:char] ` The `markChar` property returns or sets the character used to mark a menu item. If the item has no mark, `the markChar` returns` empty`.  Otherwise, it returns the character.

Setting the `markChar` of a menu item to a character also marks the item, that is, sets its `checkMark` property to true. 

 The default character used to mark menu items is the check mark, a character equal to` numToChar(18)`. It prints in the Chicago font:  


## Examples

```
-- numToChar(19) produces a diamond character in Chicago:
set the markChar of menuItem "New" of menu "File" to numToChar(19)
set the markChar of menuItem 2 of menu 2 to numToChar(19)
set the markChar of second menuItem of second menu to numToChar(19)
```

## Demo Script

```
on mouseUp
  if there is a menu "Reference"
  then set the <b>markChar</b> of menuItem 1 of menu "Reference" to ¬
  numToChar(240) -- the Apple symbol in Chicago and some other fonts
end mouseUp
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
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
