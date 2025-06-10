---
title: mouseDoubleClick
card_id: 96465
modified: yes
---

# mouseDoubleClick

`mouseDoubleClick`

Handler:

<code><pre>
on mouseDoubleClick
    <i>statements</i>
end mouseDoubleClick
</pre></code>


HyperCard sends this message to a button, field, or card after the mouse is clicked twice at the same place. When the message is sent, it's the <u>only</u> one sent during the second click;  there's no <code>mouseDown</code>, <code>mouseStillDown</code>, or <code>mouseUp</code> message sent after the first <code>mouseUp</code>.

For HyperCard to send this message, the following conditions must all be true:

(a) The downstroke of a second click follows the downstroke of a previous click within the double-click speed set in the Mouse control panel; <u>and </u> (b) the second click occurs within four pixels of the first; <u>and</u>

(c) the second click occurs within the same object as the first.

If the user clicks repeatedly at the same location faster than the double-click speed set in the Mouse control panel, HyperCard treats each odd-numbered click as a first click and each even-numbered click as a second click.

## Placeholders

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [mouseClick](/HyperTalkReference/functions/mouseClick)
* [mouseDown](/HyperTalkReference/systemmessages/mouseDown)
* [mouseStillDown](/HyperTalkReference/systemmessages/mouseStillDown)
* [mouseUp](/HyperTalkReference/systemmessages/mouseUp)
