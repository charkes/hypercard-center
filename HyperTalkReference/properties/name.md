---
title: name
card_id: 77648
modified: yes
---

# name

```
the [<i>adjective</i>] name of <i>object</i>
the [long] name of HyperCard

set [the] name of <i>object</i> to <i>text</i>
set [the] name of [<i>menuItem</i> of] <i>menu</i> ¬
   to <i>text</i>
get [the] [English] name of ¬
   [<i>menuItem</i> of] <i>menu</i>
```


The` name `property returns or sets the name of an object, menu item, or menu.  If the element doesn't have a name,` the name `returns the ID of the object instead.

`the long name of HyperCard ` returns the full path to HyperCard:

`myDisk:Desktop Folder:HyperCard Folder:HyperCard`

You can use the adjective` English `to determine the names of menus and menu items if you're using a localized version of HyperCard:

```
if the English name of menuItem 5  ¬
   of menu "Edit" is "Paste"...
```


The adjectives` abbreviated`,` long`, and` short `return various forms of an object’s name (click Demo Script to see examples).

Note:` the abbreviated name `is the same as` the name`.

## Examples

```
the short name of button 1
the abbreviated name of bkgnd button 4
the abbrev name of bkgnd button 4
the abbr name of bkgnd button 4
the name of card field 1 of last card
the long name of me
the name of menuItem 1 of menu 2
the name of first menuItem of menu "File"

set the name of button 1 to "Hide field"
set the name of this card to line 1 of field "Title"
set the name of menuItem 1 of menu "File" to "Trouble"

if the English name of menuItem 5 of menu "Edit" is not "Paste"...
```

## Demo Script

```
on nameDemo
   answer "The short name of card id 86868 is:" & return & ¬
   (the <b>short name</b> of card id 86868) & return & return &¬
   "The abbreviated name is:" & return &¬
   (the <b>abbr name</b> of card id 86868) & return & return &¬
   "The name is:" & return &¬
   (the <b>name</b> of card id 86868) & return & return &¬
   "The long name is:" & return &¬
   (the <b>long name</b> of card id 86868)
end nameDemo
```

## Placeholders

[embed:HelpExtras/Placeholders/adjective.md]

[embed:HelpExtras/Placeholders/object.md]

[embed:HelpExtras/Placeholders/text.md]

[embed:HelpExtras/Placeholders/menuItem.md]

[embed:HelpExtras/Placeholders/menu.md]

## Related Topics

* [ID ](/HyperTalkReference/properties/ID)
* [longWindowTitles](/HyperTalkReference/properties/longWindowTitles)
* [number (property)](/HyperTalkReference/properties/number-property)
