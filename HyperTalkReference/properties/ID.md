---
title: ID 
card_id: 73264
modified: yes
---

# ID 

```
the ID of <i>button</i>
the ID of <i>field</i>
the [<i>adjective</i>] ID of <i>card</i>
the ID of <i>bkgnd</i>
the ID of <i>menu</i>
the ID [of HyperCard]
the ID of <i>window</i>
```


The` ID `property returns the permanent ID number of any button, field, card,  background, window, or menu in the current stack.

The` ID `of HyperCard is` WILD`.

The` ID `of a standalone application is its creator code.

All objects except stacks have IDs. You <u>can’t</u> change the ID number of an object, window, or menu.

If an object doesn’t have a name, HyperCard returns the` ID `instead.

The adjectives` abbreviated`,` long`, and` short `return various forms of a card’s ID.  (Click Demo Script.)

## Examples

```
if the id of button 1 is "8934" then...
get the id of bkgnd field 2
put the id of this card after theList
get the id of this background
get the id of HyperCard -- returns WILD
get the id of the last menu
```

## Demo Script

```
on IDDemo

  put "The short ID of this card is:" & return & ¬
  the <b>short</b> <b>ID</b> of this card & return & return & ¬
  "The ID is:" & return & ¬
  the <b>ID</b> of this card & return & return & ¬
  "The long ID is:" & return & ¬
  the <b>long</b> <b>ID</b> of this card & return into theAnswer

  answer theAnswer
end IDDemo
```

## Placeholders

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/adjective.md]

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/bkgnd.md]

[embed:HelpExtras/Placeholders/menu.md]

[embed:HelpExtras/Placeholders/window.md]

## Related Topics

* [name](/HyperTalkReference/properties/name)
* [number (property)](/HyperTalkReference/properties/number-property)
