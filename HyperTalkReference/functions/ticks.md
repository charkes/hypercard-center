---
title: ticks
card_id: 66203
---

# ticks

<code><pre>
the ticks 
</pre></code>

Value returned: an integer equal to the number of ticks since the Macintosh was turned on or restarted. (One tick equals one-sixtieth of a second.) 


## Demo Script

<code><pre>
on ticksDemo
  put 0 into total
  put <b>the ticks</b> into startTicks
  repeat with number = 1 to 100
    set cursor to busy
    add number to total
  end repeat
  put <b>the ticks</b> - startTicks into totalTime
  answer "The sum of numbers 1 to 100 is" && total & return &¬
  "It took" && totalTime && "ticks to figure out."
end ticksDemo
</pre></code>

## Related Topics

* [seconds](/HyperTalkReference/functions/seconds)
* [time](/HyperTalkReference/functions/time)
* [wait](/HyperTalkReference/commands/wait)
