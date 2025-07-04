---
title: multipleLines
card_id: 100041
---

# multipleLines

 `set `[`the`]<code> multipleLines of [ph:field] ¬  to [ph:trueOrFalse]

</code>The `multipleLines` property returns or sets whether a user can extend the range of highlighted lines in a [ph:list field] . 

When `the multipleLines` is` true`, the user can extend highlighted lines either by shift-clicking any point before or after the insertion point in a field or by dragging through text. 

 `MultipleLines `appears as the  “Multiple Lines” option in the Field Info dialog box, where it is disabled if `autoSelect `is set to false. 

To learn which lines are selected, get the` selectedLine of [ph:field`].  

To learn the contents of those lines, get the` selectedText of [ph:field`].  

To preselect lines, use    `select line x [to y] of [ph:field`] 


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
