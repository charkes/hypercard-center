### bkgnd

A HyperTalk expression that identifies a background by name, number, or id,  using one of the following forms:

```
bkgnd id [ph:posInteger]
bkgnd [ph:text] -- name
bkgnd [ph:posInteger] -- number
[ph:ordinal] bkgnd
[ph:position] bkgnd
```

For example:

```
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
```

From within a background script, the term `me` refers to that background.

When a background receives a the message `[the] target`, that message is referring to the background.

See also: `[ph:card]` 
