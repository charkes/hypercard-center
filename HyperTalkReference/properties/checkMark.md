---
title: checkMark
card_id: 69523
---

# checkMark

` set `[`the`]` checkMark of [ph:menuItem] of ¬     [ph:menu] to [ph:trueOrFalse] ` The `checkMark` property returns or sets whether a check-mark character appears in front of a menu item.

It uses the  character, `numToChar(18),` as the default check-mark character. Click Related Topics for information about the `markChar` property, which lets you use characters other than the check mark. 


## Examples

```
set the checkMark of menuItem 1 of menu "File" to true
set the checkMark of first menuItem of menu 2 to false
set the checkMark of menuItem "Open Stack..." of second menu to true
```

## Demo Script

```
on mouseUp
  if there is a menu "Reference"
  then set the <b>checkMark</b> of menuItem 1 of menu "Reference" to ¬
       not(the <b>checkMark</b> of menuItem 1 of menu "Reference")
end mouseUp
```

## Related Topics

* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [menus](/HyperTalkReference/functions/menus)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
