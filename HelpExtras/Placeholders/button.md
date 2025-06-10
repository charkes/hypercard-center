### button

<b>HyperTalk Definition </b> An expression that identifies a button by name, number, or id, using one of the following forms:

[<code>card</code>] <code>button id [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> </code>[<code>card</code>] <code>button [ph:text]</code> [<code>of [ph:card</code>] ]<code> -- name </code>[<code>card</code>] <code>button [ph:posInteger]</code> [<code>of [ph:card</code>] ]<code> [ph:ordinal] </code>[<code>card</code>] <code>button</code> [<code>of [ph:card</code>] ]<code>

bkgnd</code> <code>button id [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> bkgnd button [ph:text] </code>[<code>of [ph:card</code>] ]<code> -- name bkgnd button [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> [ph:ordinal] bkgnd button </code>[<code>of [ph:card</code>] ]<code> </code> For example:

<code><pre>
card button id 3894
card button "Return"
card button 1
first card button
bkgnd button 2 of card 2
last bkgnd button
</pre></code>

When used inside a button script: <code><pre>
me
</pre></code>

When a button receives a message: <code><pre>
[the] target
</pre></code>

A button can also be referred to as a [ph:part] when you’re talking about its position among all buttons and fields within the same card or background.

<b>AppleScript Definition </b> An expression that identifies a button by name, number, or id, using the same forms as HyperTalk except that “background” must be used in place of “bkgnd”. 