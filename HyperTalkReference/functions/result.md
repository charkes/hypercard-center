---
title: result
card_id: 62431
---

# result

<code><pre>
the result 
</pre></code>

Values returned: 

• the value set by a <code>return</code> keyword     during the execution of  a message

• <code>empty </code>if most<code> </code>commands succeed;      otherwise, a message string 

In handlers, it’s usually best to test a command with an expression such as <code><pre>

if the result is not empty then ...
</pre></code>

That way, the handler doesn’t rely on the specific value of a string.

Click Related Topics for more information about the value returned by <code>the result</code> for each command. 


## Examples

```
go card "ZZ" 
if the result is not empty then ... -- didn't go there

find "XZZ" in field "Title"
if the result is not empty then ... -- didn't find it
```

## Demo Script

<code><pre>
<code><pre>
on resultDemo
 find "Pat, Jim, Eric, and Eli" in bkgnd field "title"
 answer "Pat, Jim, Eric, Eli:" && the <b>result</b>
 go to card "Pat, Jim, Eric, and Eli"
 answer "Pat, Jim, Eric, and Eli:" && the <b>result</b>
end resultDemo
</pre></code>
</pre></code>

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
