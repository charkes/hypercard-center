### bkgnd

A HyperTalk expression that identifies a background by name, number, or id,  using one of the following forms:

<code><pre>
bkgnd id [ph:posInteger]
bkgnd [ph:text] -- name
bkgnd [ph:posInteger] -- number
[ph:ordinal] bkgnd
[ph:position] bkgnd
</pre></code>


For example: <code><pre>

bkgnd id 3894
bkgnd "Index"
bkgnd 1
prev bkgnd
previous bkgnd
next bkgnd
this bkgnd
first bkgnd
last bkgnd
middle bkgnd
any bkgnd
</pre></code>

From within a background script, the term <code>me </code>refers to that background. <code><pre>
</pre></code>

When a background receives a the message <code>[the] target, </code>that message is referring to the background.

See also:<code> [ph:card]</code> 