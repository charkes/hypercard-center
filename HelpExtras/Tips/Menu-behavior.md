---
title: Menu behavior
card_id: 34927
---

### Menu behavior

You can handle menu events from your scripts in two ways.

First, HyperCard sends a `doMenu` message, so you can write a `doMenu` handler to respond to the event.

Second, if you do not handle the `doMenu` message, HyperCard checks the `menuMessage` property of the menu item. If it finds a message there, HyperCard sends this message to the current card. So you can also write a handler for this message to respond to the event.

Note: Because HyperCard sends the `doMenu` message first, a `doMenu` handler will always override a specific handler meant to handle a` menuMessage`.

Other tips:

*You can just `disable` or `delete` the     Tools, Patterns, Font, and Apple menus.     HyperCard does not allow other     operations on these menus, such as     setting a Command character. (But you can      modify the first item in the Apple     menu.)

* You can use the` set`,` get`,` put`,` delete`,`  `   `enable`, and `disable` commands with     menus that aren’t currently visible     (perhaps because the menu bar is     hidden, the user level is set too low, or a     different tool is chosen).

* For HyperCard’s standard menus, the    ` doMenu `command always works, even if     an item is deleted or not available. For     example, the following handler will quit     HyperCard:

```
 on mouseUp
   delete menuItem "Quit HyperCard" ¬
   from menu "File"
   doMenu "Quit HyperCard"
 end mouseUp
```

* If you add a menu item with the  same      name  as one of HyperCard’s standard      menu items, the new item inherits the      same behavior as the standard item;      but HyperCard will not check, enable, or      disable the item automatically. 