---
title: marked
card_id: 76367
---

# marked

`set [the] marked of [ph:card] to [ph:trueOrFalse]`

The `marked` property returns or sets whether a card is marked. It corresponds to the Card Marked check box in a Card Info dialog box.

You can operate on the set of marked cards with commands such as `print`, `go`, `show`, and `sort`. 

## Examples

```
set the marked of this card to true
set the marked of last card of next background to false
set the marked of marked card 1 to false
```

## Related Topics

* [mark](/HyperTalkReference/commands/mark)
* [unmark](/HyperTalkReference/commands/unmark)
