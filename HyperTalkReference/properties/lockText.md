---
title: lockText
card_id: 75848
---

# lockText

<code> set </code>[<code>the</code>]<code> lockText of [ph:field] ¬     to [ph:trueOrFalse]

</code>The <code>lockText</code> property returns or sets whether the user can edit the text within a specified field. It corresponds to the Lock Text check box in a Field Info dialog box. The default value is false (meaning the field is unlocked). 

 When a field is locked, it can receive the system messages <code>mouseDown</code>,<code> mouseDoubleClick, mouseStillDown</code>, and<code> mouseUp</code> when the user clicks it.

Before a field can act as a[ph: list field],  its <code> lockText </code>property must be set to true. 


## Examples

```
set the lockText of card field 1 to true
set the lockText of the target to false -- if the target is a field
set the lockText of me to true -- if in a field script
```

## Related Topics

* [autoSelect](/HyperTalkReference/properties/autoSelect)
