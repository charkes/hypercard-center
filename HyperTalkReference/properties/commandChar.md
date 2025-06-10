---
title: commandChar
card_id: 70039
---

# commandChar

<code> set </code>[<code>the</code>]<code> commandChar of [ph:menuItem] ¬     of [ph:menu] to [ph:char]

</code>The <code>commandChar</code> property returns or sets the character that you'd press with the Command key as the keyboard shortcut (commonly called the Command-key equivalent) for a menu item.  

If the menu item has no Command-key equivalent, the property returns<code> empty</code>. Otherwise, it returns the character. 

If more than one menu item use the same command character, the menu item on the menu farther to the right takes precedence.

## Examples

```
set the commandChar of menuItem 3 of menu "Help" to "?"

get the cmdChar of second menuItem of menu "File"
if it is "O" then ...
```

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menus](/HyperTalkReference/functions/menus)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
