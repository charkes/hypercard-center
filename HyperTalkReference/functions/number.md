---
title: number
card_id: 59877
modified: yes
---

# number

```
the number of [card] {buttons|parts}
the number of bkgnd {buttons|parts}
the number of card fields
the number of [bkgnd] fields

the number of marked cards the number of cards [in [ph:bkgnd]] ¬
   [of this stack]
the number of bkgnds [of this stack]

the number of windows
the number of menus
the number of menuItems of [ph:menu]
the number of [ph:chunks] in [ph:expression]
```

Values returned: A non-negative integer equal to one of the following:

* total number of buttons <u>or</u> fields on the current card or background

* total number of parts (buttons <u>and</u> fields combined) on the current card      or background

* total number of marked cards, cards in a specific background, cards in an entire stack, or backgrounds in a stack

*  number of all the windows (including built-in palettes and external windows) in HyperCard

*  number of menus in the menu bar or the number of menu items in a specified menu

*  total number of characters, words, items, or lines in the value of any HyperTalk expression (treated as text)

## Examples

```
-- Count the menu items in a menu:
the number of menuItems of menu 2
the number of menuItems of second menu
the number of menuItems of menu "File"

-- Count the number of objects:
the number of card fields
the number of background buttons
the number of cards
the number of cards of this background
the number of backgrounds
the number of parts
the number of background parts

-- Count the number of chunks in text (including containers):
the number of chars in card field 2
the number of lines in the stacksInUse

-- Do something based on the number of cards:
repeat with i = 1 to the number of cards of this background
   statements
end repeat

repeat with i = 1 to the number of marked cards
   statements
end repeat
```

## Demo Script

```
on numberOfChunks
  get bkgnd field "Demo Script"
  answer "There are" && the <b>number</b> of lines in it && ¬
  "lines and" && the <b>number</b> of words in it && "words and" && ¬
  the <b>number</b> of characters in it && "characters in this handler."
end numberOfChunks
```

## Related Topics

* [ID ](/HyperTalkReference/properties/ID)
* [name](/HyperTalkReference/properties/name)
* [number (property)](/HyperTalkReference/properties/number-property)
