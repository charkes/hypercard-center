---
title: multipleLines
card_id: 100041
---

# multipleLines

 <code>set </code>[<code>the</code>]<code> multipleLines of [ph:field] ¬  to [ph:trueOrFalse]

</code>The <code>multipleLines</code> property returns or sets whether a user can extend the range of highlighted lines in a [ph:list field] . 

When <code>the multipleLines</code> is<code> true</code>, the user can extend highlighted lines either by shift-clicking any point before or after the insertion point in a field or by dragging through text. 

 <code>MultipleLines </code>appears as the  “Multiple Lines” option in the Field Info dialog box, where it is disabled if <code>autoSelect </code>is set to false. 

To learn which lines are selected, get the<code> selectedLine of [ph:field</code>].  

To learn the contents of those lines, get the<code> selectedText of [ph:field</code>].  

To preselect lines, use    <code>select line x [to y] of [ph:field</code>] 


## Examples

```

get the multipleLines of field 6

if the multipleLines of field list is true
then answer "You may choose three items in this list."
```

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
* [lockText](/HyperTalkReference/properties/lockText)
* [select](/HyperTalkReference/commands/select)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
* [selectedText](/HyperTalkReference/functions/selectedText)
