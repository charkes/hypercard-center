---
title: cantModify
card_id: 69105
---

# cantModify

<code><pre>
set [the] cantModify of [ph:stack] ¬
    to [ph:trueOrFalse]
</pre></code>

The <code>cantModify</code> property returns or sets whether a stack can be changed in any way. It corresponds to the Can’t Modify check box in the Protect Stack dialog box.

Setting the <code>cantModify</code> of a stack to <code>true </code>selects both the Can’t Modify Stack check box and the Can’t Delete Stack check box in the Protect Stack dialog box.  When <code>cantModify</code> is true, a padlock appears in the menu bar. 

 The default value is <code>false</code> (meaning that the card, background, or stack can be modified). 


## Examples

```
set the cantModify of this stack to true
set the cantModify of stack "My Kiosk" to true
```

## Demo Script

<code><pre>
on cantModifyDemo
   -- Test whether a stack is locked from the Finder, is on locked
   -- media, or is in a read-only folder on a shared volume. If it is,
   -- you can't set cantModify to false
   set <b>cantModify</b> of this stack to false
   if <b>cantModify</b> of this stack is true then
      answer "This stack is locked or is on locked media."
   else answer "This stack is not locked."
end cantModifyDemo
</pre></code>

## Related Topics

* [cantDelete](/HyperTalkReference/properties/cantDelete)
* [userModify](/HyperTalkReference/properties/userModify)
