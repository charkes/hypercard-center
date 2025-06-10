### chunk

One of the following forms (or combinations thereof):

[ph:<code>ordinal] character character [ph:posInteger] </code>[<code>to [ph:posInteger</code>] ]<code> <u> [ph:</u>ordinal] word word [ph:posInteger] </code>[<code>to [ph:posInteger</code>] ]<code> <u> [ph:</u>ordinal] item item [ph:posInteger] </code>[<code>to [ph:posInteger</code>] ]<code> <u> [ph:</u>ordinal] line line [ph:posInteger] </code>[<code>to [ph:posInteger</code>] ]

For example:

<code><pre>
first character
second item
middle line
character 1
char 1 to 10
word 3
item 5 to (the number of items of me)
line 1 to 10
char 1 to 10 of word 2 to 4 of ¬
line 3 to 6
</pre></code>

A chunk combined with <code>of</code> and a container is called a[ph: chunk expression.]  For example: <code><pre>

line 1 of card field "index"
</pre></code>


<b>Important</b>: You can’t combine a stack name with a chunk expression—you can only refer to a chunk in the current stack. 