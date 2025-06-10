---
title: markChar
card_id: 76221
---

# markChar

<code> set </code>[<code>the</code>]<code> markChar of [ph:menuItem] of ¬     [ph:menu] to [ph:char] </code> The <code>markChar</code> property returns or sets the character used to mark a menu item. If the item has no mark, <code>the markChar</code> returns<code> empty</code>.  Otherwise, it returns the character.

Setting the <code>markChar</code> of a menu item to a character also marks the item, that is, sets its <code>checkMark</code> property to true. 

 The default character used to mark menu items is the check mark, a character equal to<code> numToChar(18)</code>. It prints in the Chicago font:  


## Examples

```
-- numToChar(19) produces a diamond character in Chicago:
set the markChar of menuItem "New" of menu "File" to numToChar(19)
set the markChar of menuItem 2 of menu 2 to numToChar(19)
set the markChar of second menuItem of second menu to numToChar(19)
```

## Demo Script

<code><pre>
on mouseUp
  if there is a menu "Reference"
  then set the <b>markChar</b> of menuItem 1 of menu "Reference" to ¬
  numToChar(240) -- the Apple symbol in Chicago and some other fonts
end mouseUp
</pre></code>

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
