### field

An expression that identifies a field by name, number, or id using one of the following forms (in AppleScript, use “background” in place of “bkgnd”):

<code>card</code> <code>field id [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> card field [ph:text] </code>[<code>of [ph:card</code>] ]<code> -- name card field [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> [ph:ordinal] card field </code>[<code>of [ph:card</code>] ]

[<code>bkgnd</code>] <code>field id [ph:posInteger] </code>[<code>of [ph:card</code>] ]<code> </code>[<code>bkgnd</code>] <code>field [ph:text]</code> [<code>of [ph:card</code>] ]<code> -- name </code>[<code>bkgnd</code>] <code>field [ph:posInteger]</code> [<code>of [ph:card</code>] ]<code> [ph:ordinal] </code>[<code>bkgnd</code>] <code>field</code> [<code>of [ph:card</code>] ]

For example:

<code><pre>
card field id 3894
card field "My Notes"
card field 1
first card field
background field 3 of card 1
</pre></code>

When used inside a field script in HyperTalk: <code><pre>
me
</pre></code>

When a field receives a message: <code>[the] target</code>

A field can also be referred to as a [ph:part] when you’re talking about its position among all buttons and fields within the same card or background. 