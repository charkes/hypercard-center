### card

An expression that identifies a card by name, number, or id using one of the following forms (in AppleScript, use “background” in place of “bkgnd”):

<code><pre>
recent card
back
forth
card id [ph:posInteger] [of [ph:bkgnd]
card [ph:text] [of [ph:bkgnd]] -- name
card [ph:posInteger] [of [ph:bkgnd]] -- number
[ph:ordinal] card [of [ph:bkgnd]]
[ph:position] card [of [ph:bkgnd]]
[ph:ordinal] marked card
[ph:position] marked card
marked card [ph:posInteger]
</pre></code>

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

When used inside a card script in HyperTalk: `me`

When a card receives a message: `[the] target`

See also: <code>[ph:button]</code> and <code>[ph:field]</code>
