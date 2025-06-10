---
title: number (property)
card_id: 77883
modified: yes
---

# number (property)

<code><pre>
the number of <i>button</i>
the number of <i>field</i>
the number of <i>card</i>
the number of <i>bkgnd</i>
the number of <i>window</i>
</pre></code>


The<code> number </code>property returns the number of a button, field, card,  background, or window. (You cannot<code> set </code>a number.) The number of a button or field determines whether it’s on top of other buttons and fields within the same layer (background or card) that contains it. Card objects are always on top of background objects.

To change the number of a button or field, select it and choose Send Farther and Bring Closer from the Objects menu, or change its<code> partNumber </code>property.

The number of a window reflects its front to back order (similar to the number of a button or field).  You can change a window's number by bringing it to the front (for example, by clicking it or by using the<code> show </code>command), or by covering it with other windows.

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

<code><pre>
<code><pre>
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
</pre></code>
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/bkgnd.md]

[embed:HelpExtras/Placeholders/window.md]

## Related Topics

* [ID ](/HyperTalkReference/properties/ID)
* [name](/HyperTalkReference/properties/name)
* [number](/HyperTalkReference/functions/number)
* [partNumber](/HyperTalkReference/properties/partNumber)
