---
title: textArrows
card_id: 84197
---

# textArrows

<code>set </code>[<code>the</code>]<code> textArrows to [ph:trueOrFalse]

</code>The <code>textArrows</code> property returns or sets whether the arrow keys move the insertion point in a field or move you through stacks.

When the <code>textArrows</code> property is false, the Right Arrow and Left Arrow keys <u>always</u> take you to the next and previous cards in the stack, and the Up Arrow and Down Arrow keys take you forward and backward through the cards you’ve already viewed. 

When the <code>textArrows</code> property is true, the arrow keys move the text insertion point around in a field that you’re editing or in the Message box; if you’re not editing, they move you through cards.

HyperCard determines the default setting for <code>textArrows</code> at startup (and when HyperCard resumes after being suspended) from the Arrow Keys in Text option on the Preferences card of the Home stack. 


## Examples

```
set the textArrows to true
```

## Related Topics

* [arrowKey](/HyperTalkReference/commands/arrowKey)
* [returnKey](/HyperTalkReference/commands/returnKey)
* [tabKey](/HyperTalkReference/commands/tabKey)
