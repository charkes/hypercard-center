---
title: time
card_id: 66404
---

# time

<code>the </code>[[ph:<code>adjective</code>] ]<code> time time() </code> Value returned: A text string representing the current time set in your Macintosh, in one of the following time formats: <code><pre>

the time           -- 9:14 AM
time()             -- 9:14 AM
the abbrev time    -- 9:14 AM
the short time     -- 9:14 AM
the long time      -- 9:14:42 AM
the English time   -- 9:14:42 AM
</pre></code>



 When HyperCard is running under System 7.1, the long, abbrev, and short forms agree with the formats set in the Date & Time Control Panel.

The form <code>the English time</code> returns the time in the form <code>[ph:hh ]:[ph:mm ]:[ph:ss]:  AM|PM</code> no matter what language the system is localized for and no matter what the settings are on the Date & Time Control Panel. 


## Examples

```
the short time
the abbreviated time
the abbrev time
the abbr time
the time
the long time
time()
```

## Demo Script

<code><pre>
<code><pre>
on clock
 show bkgnd field "Demo Field"
 put the ticks into startTicks
 put the seconds into startSeconds
 repeat until the mouseClick
   displayMessage "The time is" && the <b>time</b> & return & ¬
   "The long time is" && the <b>long</b> <b>time</b> & return & return &¬
   the seconds - startseconds && "seconds have elapsed." & return & ¬
   the ticks - startTicks && "ticks have elapsed." & return & return &¬
   spaces(20) & "Click the mouse to continue . . ."
 end repeat
 hide bkgnd field "Demo Field"
end clock
</pre></code>
</pre></code>

## Related Topics

* [convert](/HyperTalkReference/commands/convert)
* [date](/HyperTalkReference/functions/date)
* [seconds](/HyperTalkReference/functions/seconds)
* [ticks](/HyperTalkReference/functions/ticks)
* [wait](/HyperTalkReference/commands/wait)
