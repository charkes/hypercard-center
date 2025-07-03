---
title: arrowKey
card_id: 30663
modified: yes
---

# arrowKey

`arrowKey [ph:direction]`

If the global property `textArrows` is `false`, the `arrowKey` command navigates through cards:

`arrowKey left`  = go to previous card
`arrowKey right` = go to next card
`arrowKey up`    = go forward through recent cards
`arrowKey down`  = go backward through recent cards

If the global property `textArrows` is `true`, the `arrowKey` command navigates through cards unless the insertion point is in a field. Then `arrowKey` moves the insertion point within the field.

HyperCard sends the `arrowKey` command to the current card when an arrow key is pressed. The value passed to the parameter variable `[ph:direction]` is `left`, `right`, `up`, or `down`, depending on which arrow key is pressed.

To handle the `arrowKey` message, use the following form:

```
on arrowKey whichKey
   [ph:statements]
end arrowKey
```

In the above form, the parameter variable `whichKey` is set to a `[ph:direction]`.

## Examples

```
-- Option + left and right arrow keys go to prev and next marked card
on arrowKey whichKey
  if the optionKey is down then
    if whichKey is "left" then
      go previous marked card
    else if whichKey is "right" then
      go next marked card
    end if
  else pass arrowKey -- let the other arrowKey messages pass
end arrowKey
```

## Placeholders

[embed:HelpExtras/Placeholders/direction.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [textArrows](/HyperTalkReference/properties/textArrows)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
