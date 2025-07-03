---
title: select
card_id: 47006
modified: yes
---

# select

```
select empty
select [ph:button]
select [ph:field]
select text of [ph:container]
select before text of [ph:container]
select after text of [ph:container]
select [ph:chunk] of [ph:container]
select before [ph:chunk] of [ph:container]
select after [ph:chunk] of [ph:container]
```

<b>Note:</b> `[ph:container]` cannot be a variable.

The `select` command selects buttons, fields, or text.

`Select [ph:button]` selects a button as if you had chosen the Button tool and clicked it. `Select [ph:field]` selects a field as if you had chosen the Field tool and clicked it.

Note: You can’t use `select` to select hidden buttons or fields, and the user level must be set to Authoring or Scripting for `select` to work.

`Select empty` removes the current selection.  Use `select empty` instead of `click at` to deselect text or objects.

`Select text` applies to all the text in a field or in the Message box. You can select all the text or place the insertion point before the first character or after the last character of text.

`Select [ph:chunk]` applies to a specified range of text in the Message box or in a field, to one or more lines in a list field, or to a line (that is, a “menu” item) in a popup button.

In the Message box or in a field you can select the entire range of text or place the insertion point before the first character or after the last character of the range.

## Examples

```
-- Select a button or a field:
select background button id 12
select card field 1
select me

select empty

-- Set the insertion point in a field:
select before word 2 of field "syntax"
select after line 1 of first field
select after text of cd fld id 2378

-- Select a range of text in a field or msg box:
select char 1 of field "syntax"
select item 2 of field "names"
select word 4 to 9 of message box
select text of me -- from a script
select text of target -- from a script
select line 1 of me -- from a script
select line 3 to 6 of field "Choices" -- in a list field

-- Select a line in a pop-up menu:
select line 3 of button "Maps"
```

## Demo Script

```
on selectDemo
  -- select an object and move it:
  <b>select</b> bkgnd button "Run the Script"
  set dragSpeed to 60
  drag from 386,255 to 386,75
  wait 1 second
  domenu "undo"


  -- select a range of characters:
  set cursor to watch
  <b>select</b> char 181 to 210 of bkgnd field "Demo Script"
  wait 2 seconds
  <b>select</b> empty
end selectDemo
```

## Placeholders

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/container.md]

[embed:HelpExtras/Placeholders/chunk.md]

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
* [multipleLines](/HyperTalkReference/properties/multipleLines)
* [selectedChunk](/HyperTalkReference/functions/selectedChunk)
* [selectedField](/HyperTalkReference/functions/selectedField)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
* [selectedLoc](/HyperTalkReference/functions/selectedLoc)
* [selectedText](/HyperTalkReference/functions/selectedText)
