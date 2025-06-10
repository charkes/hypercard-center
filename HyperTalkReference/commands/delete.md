---
title: delete
card_id: 34478
---

# delete

<code><pre>
delete [ph:chunk] of [ph:container]
delete
</pre></code>

[[ph:<code>menuItem] of
</pre></code>

]<code> <i>menu
</pre></code>

</i> <code>delete </code>[[ph:<code>menuItem] from</code>]<code> [ph:menu</code>] <code>delete </code>{[ph:<code>button</code>] | [ph:<code>field</code>]  |[ph:<code>part</code>] }


The <code>delete</code> command removes text from a container, menu items from a menu,  menus from the menu bar, and buttons or fields from the current card or background. 

When you use the form <code>delete [ph:part</code>] , <code> deleteButton </code>or <code>deleteField</code> is sent to the object that's being deleted. 

You can't use this command to delete a [ph:<code>part</code>]  anywhere except on the current card.

Note: Using <code>delete</code> to delete a line is not the same as putting <code>empty</code> into the line: <code>delete</code> removes the final <code>return</code> character as well as the text, while putting <code>empty</code> into the line just removes the text. 


## Examples

```
delete item 3 of line 1 of field "Expenses"
delete line 5 of button "Text Holder"

put " this has a space" into theText
delete character 1 of theText

delete menu "File"
delete menu 2
delete second menu

delete menuItem "New" from menu "File"
delete menuItem 2 from menu 2
delete second menuItem from second menu

delete button 1
delete last card field
delete background button id 1234
delete last background part
```

## Demo Script

<code><pre>
<code><pre>
on surpriseDelete
 -- appropriate surprise with style
 set the cantModify of this stack to true -- to easily restore the text
 find string "ropriate surprise with sty"
 wait 1 sec
 <b>delete</b> the foundChunk
 wait 1 sec
 set cantModify of this stack to false
end surpriseDelete
</pre></code>
</pre></code>

## Related Topics

* [put](/HyperTalkReference/commands/put)
