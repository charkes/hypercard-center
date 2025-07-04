---
title: hilite
card_id: 72540
---

# hilite

```
set [the] hilite of [ph:button] ¬
     to [ph:trueOrFalse]
```

The `hilite` property returns or sets whether a button is highlighted (shown in inverse video).  

With check boxes and radio buttons, `hilite` determines whether the button is selected.

If a button belongs to a [ph:family] and its `hilite` property is set to `true` from a script, the `hilite` property of each of the other buttons in the family is set to` false`.

(Click Tips to see a list of synonyms you can use for `hilite`.)

## Examples

```
set the hilite of bkgnd button 1 to true

set the hilite of card button id 37 to ¬
not (the hilite of card button id 37)
```

## Demo Script

```
on hiliteDemo
 flashButton "bkgnd btn id 61",3
 flashButton "bkgnd btn id 57",3
 flashButton "bkgnd btn id 58",3
end hiliteDemo
on flashButton whichBtn, howManyTimes
 repeat for (howManyTimes * 2)
   set the <b>hilite</b> of whichBtn to not the <b>hilite</b> of whichBtn
 end repeat
end flashButton
```

## Related Topics

* [autoHilite](/HyperTalkReference/properties/autoHilite)
* [sharedHilite](/HyperTalkReference/properties/sharedHilite)
