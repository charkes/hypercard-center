---
title: dontSearch
card_id: 70576
---

# dontSearch

`set `[`the`]` dontSearch of [ph:field] ¬     to [ph:trueOrFalse] set `[`the`]` dontSearch of [ph:card] ¬     to [ph:trueOrFalse] set `[`the`]` dontSearch of [ph:bkgnd] ¬     to [ph:trueOrFalse] ` The `dontSearch` property returns or sets whether HyperCard’s `find` command will look for matches in a field, card, or background. It corresponds to the Don’t Search check box in the Field Info, Card Info, and Background Info dialog boxes. 


## Examples

```
set the dontSearch of bkgnd field 1 to true

set the dontSearch of this card to false

set the dontSearch of bkgnd "Index" to true
```

## Related Topics

* [find](/HyperTalkReference/commands/find)
