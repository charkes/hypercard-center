---
title: convert
card_id: 33535
modified: yes
---

# convert

```
convert {[ph:value] |[ph:container]}[from  ¬
   [ph:formatName]  [and [ph:formatName]]] ¬
   to [ph:formatName] [and [ph:formatName]]
```

The `convert` command changes a value expressed as a valid date, time, or date and time format to another format.

You use `and [ph:formatName] `in combination with the first `[ph:formatName]` to convert a value to any two formats (often the date and time).

The form `convert [ph:value] to [ph:formatName]` returns the converted `[ph:value` in the local variable `it`. The form `convert [ph:container] to [ph:formatName]` converts a value in a chunk or `[ph:container]` (including variables) and places the result in that chunk or container.

You use the form `from [ph:format]` in situations where you don't want HyperCard to do the conversion automatically.

There are four types of date formats:

* `seconds`, a positive integer equal to the number of seconds since 12:00    midnight on January 1, 1904

* `dateItems`, a comma-delimited list of seven positive integers equal to the    following values: `year`, `month`, `day`, `hour`, `minute`,   `second`, `dayNumber` where `dayNumber 1 = Sunday` and  `7 = Saturday`.

* date, which has one of three formats:
** `[dayName,] monthName, day, year`
**  `month/day/year`
**  `month-day-year`

where `dayName` = `Sunday`, `Sun`,   `Monday`, `Mon`, `Tuesday`, `Tue`,   `Wednesday`, `Wed`, `Thursday`, `Thur`,   `Friday`, `Fri`, `Saturday`, or `Sat`

`monthName` = `January`, `Jan`, `February`, `Feb`, `March`, `Mar`, `April`,   `Apr`, `May`, `June`, `Jun`, `July`, `Jul`,   `August`, `Aug`, `September`, `Sep`,   `October`, `Oct`, `November`, `Nov`,   `December`, or `Dec`

* `time`,  which has the following format: `hour:minute[:second] [timeOfDay]`   where `timeOfDay` = `am` or `pm`

You can precede the format names `date` and `time` with an optional [ph:adjective],  producing the following formats:

```
abbrev date  Fri, Jun 15, 1990
long date    Friday, June 15, 1990
short date   6/15/90

abbrev time  3:30 PM
long time        3:30:00 PM
short time       3:30 PM
```

Note: HyperCard can handle dates from 1/1/1000 to 12/31/9999 in all formats. It handles dates from 1/1/1 to 12/31/9999 only in the `dateItems` or `seconds` format. If you try to convert an invalid date (such as `"Friday, May 50, 1990"`), HyperCard sets the HyperTalk function `the result` to `"Invalid date."`

When System 7.1 is running, HyperCard uses the date and time settings from the Date & Time Control Panel.

## Examples

```
convert "1/1/1960" to seconds -- the result goes into the variable it
convert "1/1/1960" to seconds and long date
convert (the seconds - startSeconds) to abbreviated time

convert bkgnd field "date" to seconds -- the result goes into the field
convert last word of field "Info" to short date

convert totalTime to abbreviated time -- the result goes into totalTime

convert field 1 from date to dateItems
convert myVar from seconds to long date
convert card field "Date and Time" from date and time to dateItems
```

## Demo Script

```
on daysOld
  repeat until birthTime is a date
    put "What is your birthdate?" after sayIt
    ask sayIt with the short date
    if (it is empty) OR (the result is "Cancel") then exit daysOld
    put it into birthTime
    if birthTime is not a number
    then put birthTime && "is not a valid date." & return into sayIt
  end repeat
  <b>convert</b> birthTime to seconds -- change birthTime to seconds
  <b>convert</b> the date to seconds  -- get the current date
  put (it - birthTime) / 86400 into daysOld   -- 86400 seconds in 1 day
  <b>convert</b> birthTime to long date
  answer "You were born on" && birthTime & ", and you are currently" &&¬
  daysOld && "days old."
end daysOld
```

## Related Topics

* [date](/HyperTalkReference/functions/date)
* [time](/HyperTalkReference/functions/time)
