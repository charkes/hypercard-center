---
title: commandKey
card_id: 54096
---

# commandKey

<code><pre>
the commandKey
the cmdKey
</pre></code>

Value returned: either of the constants<code> up </code>or <code>down,</code> depending on whether the Command key is up or down 


## Examples

```
if the commandKey is up then ...

if (the mouse is down) or (the commandKey is down) then ...

wait until the cmdKey is down
```

## Demo Script

<code><pre>
on commandKeyIs
  -- Hold down the Command key when you click Run the Script.
  answer "The Command key is:" && the <b>commandKey</b>
end commandKeyIs
</pre></code>

## Related Topics

* [commandKeyDown](/HyperTalkReference/commands/commandKeyDown)
