### field

An expression that identifies a field by name, number, or id using one of the following forms (in AppleScript, use “background” in place of “bkgnd”):

<code><pre>
card field id [ph:posInteger] [[of] [ph:card]]
card field [ph:text] [of [ph:card]]<code> -- name
card field [ph:posInteger] [of [ph:card]]
[ph:ordinal] card field [of [ph:card]]

[bkgnd] field id [ph:posInteger] [of [ph:card]]
[bkgnd] field [ph:text] [of [ph:card]] -- name
[bkgnd] field [ph:posInteger] [of [ph:card]]
[ph:ordinal] [bkgnd] field [of [ph:card]]

For example:

<code><pre>
card field id 3894
card field "My Notes"
card field 1
first card field
background field 3 of card 1
</pre></code>

When used inside a field script in HyperTalk: `me`

When a field receives a message: `[the] target`

A field can also be referred to as a [ph:part] when you’re talking about its position among all buttons and fields within the same card or background.
