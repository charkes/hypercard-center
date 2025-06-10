---
title: Constants
card_id: 91279
modified: yes
---

# Constants

=== down

Equal to the literal<code> "down"</code>.

<code>if the mouse is down then exit repeat</code>

=== empty

Equal to the literal<code> "" </code>(the null string)

<code>if it is empty then exit askTheUser</code>

=== false

The opposite of<code> true</code>; equal to the literal<code> "false" </code>

`if the hilite of button 1 is false then mark this card`

=== formFeed

Equal to<code> numToChar(12)</code>, which starts a new page in some file formats.

<code>write formFeed to file "My Info"</code>

=== lineFeed

Equal to<code> numToChar(10)</code>, which starts a new line in some file formats.

<code>write lineFeed to file "My Info"</code>

=== pi

Equal to the mathematical value pi to 20 decimal places:

<code>3.14159265358979323846</code>

=== quote

Equal to the double quotation mark character:`"`

`get "stack" && quote & "Home" & quote --it now contains the string: stack "Home" go it`

=== return

Equal to<code> numToChar(13)</code>.

<code><pre>
put return after field 1
write return & return to file "Data"
</pre></code>


=== space

Equal to<code> numToChar(32)</code> or the literal<code> " "</code>.

<code><pre>
if theCharacter is space
then exit checkActiveText
</pre></code>


=== tab

Equal to<code> numToChar(9)</code>.

<code>write tab to file "My Info"</code>

=== true

The opposite of<code> false</code>; equal to the literal<code> "true"</code>.

<code><pre>
if the hilite of button 1 is true
then unmark this card
</pre></code>


=== up

Equal to the literal<code> "up"</code>.

<code>if the mouse is up then exit repeat</code>

=== zero..ten

Equal to the numbers 0 through 10.

<code>go card one</code>

=== comma

Equal to the character <code>","</code> (<code>numToChar = 44</code>)

<code>read from file "Data" until comma</code>

=== colon

Equal to the character <code>":"</code> (<code>numToChar = 58</code>)

<code>set the itemDelimiter to colon</code>

