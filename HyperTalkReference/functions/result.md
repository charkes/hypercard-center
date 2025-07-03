---
title: result
card_id: 62431
---

# result

```
the result
```

Values returned:

* the value set by a `return` keyword during the execution of a message

* `empty` if most commands succeed; otherwise, a message string

In handlers, it’s usually best to test a command with an expression such as

```
if the result is not empty then ...
```

That way, the handler doesn’t rely on the specific value of a string.

Click Related Topics for more information about the value returned by `the result` for each command. 

## Examples

```
go card "ZZ"
if the result is not empty then ... -- didn't go there

find "XZZ" in field "Title"
if the result is not empty then ... -- didn't find it
```

## Demo Script

```
```
on resultDemo
 find "Pat, Jim, Eric, and Eli" in bkgnd field "title"
 answer "Pat, Jim, Eric, Eli:" && the <b>result</b>
 go to card "Pat, Jim, Eric, and Eli"
 answer "Pat, Jim, Eric, and Eli:" && the <b>result</b>
end resultDemo
```
```

## Related Topics

* [answer](/HyperTalkReference/commands/answer)
* [ask](/HyperTalkReference/commands/ask)
* [convert](/HyperTalkReference/commands/convert)
* [create](/HyperTalkReference/commands/create)
* [export paint](/HyperTalkReference/commands/export-paint)
* [find](/HyperTalkReference/commands/find)
* [function](/HyperTalkReference/keywords/function)
* [go](/HyperTalkReference/commands/go)
* [icon](/HyperTalkReference/properties/icon)
* [import paint](/HyperTalkReference/commands/import-paint)
* [on](/HyperTalkReference/keywords/on)
* [open](/HyperTalkReference/commands/open)
* [open printing](/HyperTalkReference/commands/open-printing)
* [open report printing](/HyperTalkReference/commands/open-report-printing)
* [print](/HyperTalkReference/commands/print)
* [return](/HyperTalkReference/keywords/return)
* [save](/HyperTalkReference/commands/save)
