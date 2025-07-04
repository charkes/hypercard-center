---
title: number (property)
card_id: 77883
modified: yes
---

# number (property)

```
the number of [ph:button]
the number of [ph:field]
the number of [ph:card]
the number of [ph:bkgnd]
the number of [ph:window]
```

The `number` property returns the number of a button, field, card,  background, or window. (You cannot `set` a number.) The number of a button or field determines whether it’s on top of other buttons and fields within the same layer (background or card) that contains it. Card objects are always on top of background objects.

To change the number of a button or field, select it and choose Send Farther and Bring Closer from the Objects menu, or change its `partNumber` property.

The number of a window reflects its front to back order (similar to the number of a button or field).  You can change a window's number by bringing it to the front (for example, by clicking it or by using the `show` command), or by covering it with other windows.

The number of a card is its position within a stack. The number of a background is the order in which the background was created. To change the number of a card or background, you must use the sort command or cut cards and paste them into different positions within the stack.

## Examples

```
the number of bkgnd button "Prev"
the number of card field id 90
the number of this card
the number of this background

if the number of this card = 1 then ...
```

## Demo Script

```
on nameDemo
 answer "The number of bkgnd field “Demo Script” is:" && ¬
 the <b>number</b> of bkgnd field "Demo Script" & return & return & ¬
 "The number of this card is:" && ¬
 the <b>number</b> of this card & return & return & ¬
 "The total number of cards in the stack is:" && ¬
 the <b>number</b> of cards & return & return & ¬
 "The number of this background is:" && ¬
 the <b>number</b> of this bkgnd
end nameDemo
```

## Related Topics

* [ID ](/HyperTalkReference/properties/ID)
* [name](/HyperTalkReference/properties/name)
* [number](/HyperTalkReference/functions/number)
* [partNumber](/HyperTalkReference/properties/partNumber)
