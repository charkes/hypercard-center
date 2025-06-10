### part

An expression that identifies a [ph:button] or [ph:field] by its ordinal position among all buttons and fields on the same [ph:card] or [ph:bkgnd].

A button's or field’s part number is available in its Info dialog box; in a script, it is available in the object’s <code>partNumber</code> property.

You can use any of these forms:

<code<pre>
[card] part [ph:posInteger]
[bg] part [ph:posInteger]
[ph:ordinal] [card]
[bg] part
</pre></code>

For example:

<code><pre>
card part 5
first card part
last background part
</pre></code>
