---
title: date
card_id: 55207
---

# date

`the [[ph:adjective]] date`
`date()`

Value returned: text string representing the current date set in your Macintosh, in the following date formats:

```
the date                  -- 12/25/93
date()                    -- 12/25/93
the abbrev date    -- Sat, Dec 25, 1993
the short date      -- 12/25/93
the long date    -- Saturday, December 25, 1993
the English date  -- Saturday, December 25, 1993
```

When HyperCard is running under System 7.1, the long, abbrev, and short forms agree with the formats set in the Date & Time Control Panel. The form `the English date` returns the date in the form `[ph:day], [ph:month] [ph:dayNumber], [ph:fullYearNumber]` using english weekdays and months no matter what language the system is localized for and no matter what the settings are on the Date & Time Control Panel.

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
