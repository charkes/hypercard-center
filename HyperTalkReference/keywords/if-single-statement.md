---
title: if (single-statement)
card_id: 26805
modified: yes
---

# if (single-statement)

<code><pre>
if <i>trueOrFalse</i> then <i>statements</i> ¬
   [else <i>statements</i>]

if <i>trueOrFalse</i>
then <i>statements</i>
[else if <i>trueOrFalse</i>
then <i>statements</i>]
[else <i>statements</i>]
</pre></code>

<br>
The single-statement<code> if </code>structure tests for a condition and executes <b>one</b> statement if the condition is true. You use the optional<code> else if </code>or<code> else </code>form to run other  blocks of code in case the  condition following<code> if </code>is false.<br>
<br>
Because each part of a simple<code> if </code>structure is limited to one statement, you don't need an<code> end if </code>statement.<br>
<br>
You can send a one-line <code>if </code>structure from the Message box.<br>

## Examples

```
if it is empty then exit myHandler

ask file "Save information to file:"
if it is empty then exit myHandler 
else saveFile it

ask file "Save information to file:"
if it is empty 
then exit myHandler 
else saveFile it
```

## Placeholders

[embed:HelpExtras/Placeholders/trueOrFalse.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Comparison operators](/HyperTalkReference/operatorsandconstants/Comparison-operators)
* [Logical operators](/HyperTalkReference/operatorsandconstants/Logical-operators)
* [Type and existence operators](/HyperTalkReference/operatorsandconstants/Type-and-existence-operators)
