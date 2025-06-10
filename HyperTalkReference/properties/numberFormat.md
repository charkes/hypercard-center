---
title: numberFormat
card_id: 78162
---

# numberFormat

<code>set </code>[<code>the</code>]<code> numberFormat to [ph:text]

</code>where <code>[ph:text]</code> is a valid number format. <code><pre>
</pre></code>

The <code>numberFormat</code> property returns or sets the precision with which the results of mathematical operations are displayed in fields and the Message box.  The following symbols specify the number format:

0  Use one zero for each digit you want     to appear. .   Use a period to indicate the position      of the decimal point, if any. 

# Use to indicate where you want      trailing digits to appear if      they have a value other than zero.  

HyperCard sets the default number format to <code>"0.######"</code> on idle.  <b>

Important</b>: <code>numberFormat</code> takes effect only when you perform a mathemat- ical operation on a number. 


## Examples

```
--For the number 2.2:
set the numberFormat to "00.00" -- displays 02.20
set the numberFormat to "0" -- displays 2
set the numberFormat to "0.######" -- displays 2.2

In the following set of statements, the Message box would display 3.14159265358979323846 because HyperCard converts the string to a number only when you perform a mathematical operation on it:

put pi into myVar
set numberFormat to "0.00"
put myVar into message box

In the next set of statements, the Message box would display 3.14 because HyperCard converts the string to a number when you add 0 to it:

put pi into myVar
add 0 to myVar
set numberFormat to "0.00"
put myVar into message box
```

## Related Topics

* [annuity](/HyperTalkReference/functions/annuity)
* [Arithmetic operators](/HyperTalkReference/operatorsandconstants/Arithmetic-operators)
* [compound](/HyperTalkReference/functions/compound)
* [cos](/HyperTalkReference/functions/cos)
* [divide](/HyperTalkReference/commands/divide)
* [multiply](/HyperTalkReference/commands/multiply)
* [sin](/HyperTalkReference/functions/sin)
* [sqrt](/HyperTalkReference/functions/sqrt)
* [tan](/HyperTalkReference/functions/tan)
