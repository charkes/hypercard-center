---
title: programs
card_id: 103709
---

# programs

<code><pre>
the programs [of machine "[ph:zone:Mac]"]
</pre></code>

Value returned: a return-delimited list of applications currently running on the same machine as HyperCard

If you use the optional form <code>of machine "[ph:zone:Mac]",</code> you get a list of Apple event-aware programs running on a remote machine.

This function requires System 7 to work. (See Demo Script.) 


## Examples

```


put the programs into card field 2

answer programs()

get the programs of machine "Zone 3:Freda's Mac"
```

## Demo Script

<code><pre>
on mouseUp
  if the systemVersion < 7.0 then
    answer "Requires System 7 or greater!"
    exit to HyperCard
  end if
  answer "The <b>programs</b> running at present are:"¬
  & return & return & the programs
end mouseUp
</pre></code>

## Related Topics

* [answer](/HyperTalkReference/commands/answer)
* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [reply](/HyperTalkReference/commands/reply)
* [request](/HyperTalkReference/commands/request)
