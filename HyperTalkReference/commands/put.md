---
title: put
card_id: 45460
modified: yes
---

# put

<code><pre>
put [ph:expression]
put [ph:expression] [ph:preposition] ¬
   [[ph:chunk] of] [ph:container]

put [ph:menuItemList] [ph:preposition] ¬
     [[ph:menuItem] of] [ph:menu] ¬
     [with menuMessages [ph:messageList]]
</pre></code>

The <code>put</code> command evaluates an expression and places the value it extracts <code>into</code>, <code>after</code>, or <code>before</code> the contents of a container.

The container can be a button, a field, a variable, the Message box, the selection, a <code>[ph:chunk]</code> expression, or a menu. If you don’t specify a container, HyperCard puts the value into the Message box, showing it if it’s hidden.

Use <code>put</code> with <code>into</code> to replace the contents of a container or menu, with <code>before</code> to place the value at the beginning of its contents, and with <code>after</code> to append the value to the end of its contents.

The lines of text that you put into a pop-up button become the items of the  menu that appears when you click the button.

Before you can add items to a menu, the menu must already exist.

The <code>[ph:menuItemList]</code> is a comma-separated list of the items you want to add to the menu. Use the single character <code>"-"</code> to get a gray line. You can put up to 64 items into a menu with a single <code>put</code> statement.

The optional <code>[ph:messageList]</code> is a comma-separated list of message names that HyperCard sends to the current card when the user chooses one of the menu items. The number of items in the <code>[ph:messageList]</code> must equal the number of items in<code> [ph:menuItemList].</code>

To skip a message name, use an empty item—a null between two commas:

<code>"myMessage 1,,myMessage 3"</code>

## Examples

```
-- These are equivalent:
put 42.5 * 675
put 42.5 * 675 into msg
put 42.5 * 675 into the Message box

put empty into It  

put "Hello" into field 1  
put "Go: " before field "WhereTo"  
put "." after last character of last word of field 3  
put the date into varName
put the clickLine into theLineClicked
put the value of the clickLine into theTextClicked
put "*" after the selection

-- Add items to a menu:
create menu "Example"
put "1,2,3,-,4,5,6" into menu "Example"
put "7" after menu "Example" with menuMessage "beep"
put "a,b,c,-" before menu "example" ¬
    with menuMessages "beep,beep 2,beep 3,empty"

-- add items to a button
put "Boston" & return & "New York" & return & "Salem" into button "Maps"
```

## Demo Script

<code><pre>
on putDemo
  get bkgndFields()
  if the number of chars of it < 255 then answer it
end putDemo

function bkgndFields
  -- Returns a return-delimited list of the bg fields
  repeat with i = 1 to the number of bkgnd fields
    <b>put</b> the short name of bg field i & return <b>after</b> theFields
  end repeat
  return theFields
end bkgndFields
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

[embed:HelpExtras/Placeholders/preposition.md]

[embed:HelpExtras/Placeholders/chunk.md]

[embed:HelpExtras/Placeholders/container.md]

[embed:HelpExtras/Placeholders/menuItemList.md]

[embed:HelpExtras/Placeholders/menuItem.md]

[embed:HelpExtras/Placeholders/menu.md]

[embed:HelpExtras/Placeholders/messageList.md]

## Related Topics

* [create](/HyperTalkReference/commands/create)
* [delete](/HyperTalkReference/commands/delete)
* [get](/HyperTalkReference/commands/get)
* [set](/HyperTalkReference/commands/set)
