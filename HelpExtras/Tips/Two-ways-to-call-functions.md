---
title: Two ways to call functions
card_id: 32809
---

### Two ways to call functions

You can call HyperTalk functions that require one or no parameter using either of the following forms:

`     the abs of -5`
`     abs(-5)`

Note: You cannot use the parentheses form to call ` the result `or` the target.`

The second form is less ambiguous than the first because it explicitly groups the parameters. Note the differences among the following:

```
the abs of -5 + 100 = 105
the abs of (-5 + 100) = 95
abs(-5) + 100 = 105
abs(-5 + 100) = 95
```


<b>Important</b>: You can use only the form  `the abs of -5 `with HyperCard’s built-in functions. Function handlers that you define must be called using parentheses:

```
get myPassword()
put myRandomNumber(10)
```

