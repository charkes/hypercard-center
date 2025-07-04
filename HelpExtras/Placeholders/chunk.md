### chunk

One of the following forms (or combinations thereof):

```
[ph:ordinal] character
character [ph:posInteger] [to [ph:posInteger]]
[ph:ordinal] word
word [ph:posInteger] [to [ph:posInteger]]
[ph:ordinal] item
item [ph:posInteger] [to [ph:posInteger]]
[ph:ordinal] line
line [ph:posInteger] [to [ph:posInteger]]
```

For example:

```
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
```

A chunk combined with `of` and a container is called a <i>chunk expression<i>.  For example: `line 1 of card field "index"`

<b>Important</b>: You can’t combine a stack name with a chunk expression—you can only refer to a chunk in the current stack.
