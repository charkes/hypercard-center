---
title: create
card_id: 34045
---

# create

<code><pre>
create menu [ph:menuName]
create stack [ph:fileName] [with [ph:bkgnd] ¬
    [in a new window]
</pre></code>

The <code>create menu</code> command makes a new menu and adds it to the menu bar.   HyperCard displays an error message if you try to create a menu that already exists.

Use the <code>put</code> command to add menu items to the new menu. (Click Related Topics for more information about <code>put</code>.)

The <code>create stack</code> command creates a new stack from within a handler without presenting the New Stack dialog box. The cards in the new stack are the same size as the cards in the current stack.

HyperCard sets the function <code>the result</code> to <code>"Couldn't create stack."</code> if it can’t create the stack; otherwise, it sets <code>the result</code> to <code>empty</code>, goes to the new stack, and sends a <code>newStack</code> message to the only card in that stack (that is, the current card).

## Examples

```
create stack "Junk"
create stack "Junk" with background "Content"

ask file "Create a stack called:"
if it is not empty then create stack it

create menu "Brass"
put "Trumpet,French Horn,Trombone,Tuba" into menu "Brass"
```

## Demo Script

<code><pre>
on createMenu
  if there is a menu "Sort" then delete menu "Sort"
  <b>create</b> menu "Sort"
  put "By name,By number,By International,-,Ascending,Descending" ¬
  into menu "Sort"
  set the checkMark of menuItem 1 of menu "Sort" to true
  set the checkMark of menuItem 5 of menu "Sort" to true
end createMenu
</pre></code>

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [menus](/HyperTalkReference/functions/menus)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
