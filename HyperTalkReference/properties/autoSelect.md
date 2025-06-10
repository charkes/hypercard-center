---
title: autoSelect
card_id: 12857
modified: yes
---

# autoSelect

<code><pre>
set [the] autoSelect of <i>field</i> ¬
     to <i>trueOrFalse</i>
</pre></code>


The<code> autoSelect </code>property sets or returns whether lines in a locked field highlight automatically in response to a<code> mouseDown </code>event and to dragging or shift-clicking.  (Such fields are called  <i>list fields</i> .<i>)</i>

The<code> autoSelect </code>property corresponds to the Auto Select check box in a Field Info dialog box.

Automatic highlighting occurs if <code> autoSelect, lockText, and dontWrap </code>are all set to<code> true</code>.

<code>AutoSelect </code>is set to false when<code> dontWrap</code> is set to false;<code> dontWrap </code>is set to true when<code> autoSelect </code>is set to true.

For<code> autoSelect </code>to affect more than one line in a locked field, that field's <code>multipleLines </code>property must also be set to<code> true</code>.

To learn which lines are selected, get the<code> selectedLine of <i>field</i></code>.  To learn the contents of those lines, get the<code> selectedText of <i>field</i></code>.  To preselect, use <code>select line x [to y] of <i>field</i></code>.

## Placeholders

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/trueOrFalse.md]

## Related Topics

* [dontWrap](/HyperTalkReference/properties/dontWrap)
* [lockText](/HyperTalkReference/properties/lockText)
* [multipleLines](/HyperTalkReference/properties/multipleLines)
* [select](/HyperTalkReference/commands/select)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
* [selectedText](/HyperTalkReference/functions/selectedText)
