---
title: date
card_id: 55207
---

# date

<code>the [[ph:adjective] ] date</code>
<code>date()</code>

Value returned: text string representing the current date set in your Macintosh, in the following date formats:

<code>the date</code>                  --<code> 12/25/93 date()</code>                      --<code> 12/25/93 the abbrev date</code>    --<code> Sat, Dec 25, 1993 the short date</code>      --<code> 12/25/93 the long date    </code>--<code> Saturday,                        December 25, 1993  the English date </code> --<code> Saturday,                        December 25, 1993</code> 

<code> </code>
When HyperCard is running under System 7.1, the long, abbrev, and short forms agree with the formats set in the Date & Time Control Panel.<code> </code> The form <code>the English date</code> returns the date in the form <code>[ph:day],[ph: month dayNumber, fullYearNumber]</code> using english weekdays and months no matter what language the system is localized for and no matter what the settings are on the Date & Time Control Panel. 


## Examples

```
the short date
the abbreviated date
the abbrev date
the abbr date
the date
the long date
date()
```

## Related Topics

* [convert](/HyperTalkReference/commands/convert)
* [time](/HyperTalkReference/functions/time)
