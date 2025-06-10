### card

An expression that identifies a card by name, number, or id using one of the following forms (in AppleScript, use “background” in place of “bkgnd”):

<code><pre>
recent card
back
forth
card id <i>posInteger
</pre></code>

</i> [<code>of <i>bkgnd
</pre></code>

</i> ]<code> card [ph:text] </code>[<code>of [ph:bkgnd</code>] ]<code> -- name card [ph:posInteger] </code>[<code>of [ph:bkgnd</code>] ]<code> -- number [ph:ordinal] card </code>[<code>of [ph:bkgnd</code>] ]<code> [ph:position] card </code>[<code>of [ph:bkgnd</code>] ]

[ph:<code>ordinal] marked card [ph:position] marked card marked card [ph:posInteger</code>]

For example:

<code><pre>
card id 3894
card "Index"
card 1 of background 1
prev card
previous card of this background
next card
this card
first card
last card
middle card
any card
first marked card
last marked card
next marked card
previous marked card
marked card 1
marked card (the number of marked cards)
</pre></code>

When used inside a card script in HyperTalk: <code><pre>
me
</pre></code>

When a card receives a message: <code><pre>
[the] target
</pre></code>

See also: <code>[ph:button</code>] <code></code> and<code> [ph:field]</code> 