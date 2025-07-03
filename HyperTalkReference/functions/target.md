---
title: target
card_id: 65969
---

# target

`the [[ph:adjective] ] target` Value returned: a text string that identifies the object that originally receives a message sent by HyperCard or by the `send` keyword. If an object does not have a name, `the target` returns its ID.

The adjectives `abbreviated`, `long`, and `short` return various forms of an object’s name as with the property `the name`. (Click Related Topics for more information about `name`.)

Note: `the abbreviated target` is the same as `the target`.

HyperTalk distinguishes between `the target` and `target`: `the target` always returns a string that identifies an object, but the single word `target` is a container.

If `the target` is a button or field, `target` refers to the contents of that button or field.  If not, `target` returns an error. 

## Examples

```
the short target
the long target
the abbreviated target
the abbrev target
the abbr target

put word 2 of the clickLine into N
select line N of the target -- a field

if the target contains "button" then ...
else if the target contains "field" then ...
```

## Demo Script

```
on whoIsTheTarget
  -- Since the Run the Script button sends a message to the demo script
  -- field, the target is set to it while this handler runs.
  answer "The target is:" && <b>the target</b>
  answer "target (a container) is:" & return & return & ¬
  char 1 to 200 of <b>target </b>-- string must be < 255 chars
end whoIsTheTarget
```

## Related Topics

* [name](/HyperTalkReference/properties/name)
* [pass](/HyperTalkReference/keywords/pass)
* [send](/HyperTalkReference/keywords/send)
