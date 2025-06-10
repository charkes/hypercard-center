---
title: doMenu
card_id: 35579
modified: yes
---

# doMenu

<code><pre>
doMenu [ph:itemName] [without dialog] ¬
   [with [ph:keys]]
doMenu [ph:itemName], [ph:menuName] ¬
   [without dialog] [with [ph:keys]]
</pre></code>

The <code>doMenu</code> command performs the action specified by the item name and menu name just as if the user chose the item directly from the menu.

<code>without dialog</code> bypasses the dialog box that would normally appear after the commands Delete Stack and Convert Stack, and, when a background field is selected, after Cut Field and Clear Field.

<code>with [ph:keys]</code>chooses the named menu command with the shift, option, and/or Command keys pressed.

To determine from a script which  keys were specified, look at <code>param(6)</code> of the original command.

HyperCard sends the `doMenu` command as a message to the current card when the user selects a menu item. <code>[ph:ItemName]</code> is the exact name of the menu item selected, and <code>[ph:menuName]</code> is the exact name of the menu that contains the menu item. To handle the `doMenu` message, use this form:

<code><pre>
on doMenu theItem,theMenu
   <i>statements</i>
end doMenu
</pre></code>

Note: A `doMenu` handler can override a `menuMessage`.

## Examples

```
doMenu "Next"

-- Add another Open Stack command:
put "Open Stack..." after menu "Go" with menuMsg "beep"
doMenu "Open Stack...", "Go" -- just beeps
doMenu "Open Stack...", "File" -- does an open stack

doMenu "Calculator" -- desk accessory from the Apple menu  
doMenu "Cut Field" without dialog -- with a bkgnd field selected

doMenu "Open Stack..." with shiftKey -- checks "New Window" checkbox
doMenu "Print Card" with shiftKey -- shows print dialog

on doMenu theItem,theMenu
  if theItem is "Quit HyperCard" then answer "Bye!" with "Later"
  pass doMenu -- all doMenu messages, including the quit, are passed
end doMenu
```

## Demo Script

<code><pre>
on mouseUp
  set cursor to watch
  <b>doMenu</b> "Background","Edit" -- view the background layer
  wait 45
  <b>doMenu</b> "Background","Edit" -- return to the card layer
end mouseUp
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/itemName.md]

[embed:HelpExtras/Placeholders/menuName.md]

[embed:HelpExtras/Placeholders/ItemName.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menus](/HyperTalkReference/functions/menus)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
