---
title: choose
card_id: 31855
---

# choose

<code><pre>
choose tool [ph:posInteger]
choose [ph:toolName] tool
</pre></code>


where [ph:<code>posInteger</code>] is between 1 and 18.

The <code>choose</code> command chooses the tool with the specified number or name from the Tools palette. 

HyperCard sends the <code>choose</code> command to the current card when you choose a tool from the Tools menu. 

HyperCard passes the word [ph:tool  ]to the first parameter variable and the tool number to the second parameter variable. You can handle the <code>choose</code> command as follows:

<code><pre>
on choose what, toolNumber
  [ph:statements]
end choose
</pre></code>


## Examples

```
choose browse tool
choose tool 1

choose button tool
choose tool 2

choose field tool
choose tool 3

choose select tool
choose tool 4

choose lasso tool
choose tool 5

choose pencil tool
choose tool 6

choose brush tool
choose tool 7

choose eraser tool
choose tool 8

choose line tool
choose tool 9

choose spray tool
choose tool 10

choose rectangle tool
choose rect tool
choose tool 11

choose round rectangle tool
choose round rect tool
choose tool 12

choose bucket tool
choose tool 13

choose oval tool
choose tool 14

choose curve tool
choose tool 15

choose text tool
choose tool 16

choose regular polygon tool
choose reg poly tool
choose tool 17

choose polygon tool
choose poly tool
choose tool 18
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [tool](/HyperTalkReference/functions/tool)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
