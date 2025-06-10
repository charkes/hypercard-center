---
title: mouseUp
card_id: 21197
---

# mouseUp

<code><pre>
mouseUp
</pre></code>

Handler:

<code><pre>
on mouseUp
  [ph:statements]
end mouseUp
</pre></code>

HyperCard sends the <code>mouseUp</code> message to a button or locked field when the user releases the mouse button[ph:and]  the pointer is inside the rectangle of the same button or field it was in when the user pressed the mouse button. 

HyperCard sends <code>mouseUp</code> to the current card when the user both presses [ph:and ]releases the mouse button while the pointer is not in the rectangle of a button or field. 


## Demo Script

<code><pre>
on <b>mouseUp</b>
  answer "Hello"
end <b>mouseUp</b>
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
* [mouse](/HyperTalkReference/functions/mouse)
* [mouseClick](/HyperTalkReference/functions/mouseClick)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
