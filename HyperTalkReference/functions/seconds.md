---
title: seconds
card_id: 63225
---

# seconds

<code><pre>
the seconds
the secs
</pre></code>

Value returned: an integer equal to the number of seconds between midnight, January 1, 1904, and the current time set in your computer 


## Demo Script

<code><pre>
on secondsDemo
  -- Check the speed of an operation
  put 0 into total
  put <b>the seconds</b> into startTime
  repeat with number = 1 to 1000
    set cursor to busy
    add number to total
  end repeat
  put <b>the seconds</b> - startTime into totalTime
  answer "The sum of numbers 1 to 1000 is" && total  &&¬
  "and it took" && totalTime && "seconds to figure this out."
end secondsDemo
</pre></code>

## Related Topics

* [convert](/HyperTalkReference/commands/convert)
* [ticks](/HyperTalkReference/functions/ticks)
* [time](/HyperTalkReference/functions/time)
* [wait](/HyperTalkReference/commands/wait)
