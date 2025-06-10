---
title: target
card_id: 65969
---

# target

<code>the </code>[[ph:<code>adjective</code>] ]<code> target </code> Value returned: a text string that identifies the object that originally receives a message sent by HyperCard or by the <code>send</code> keyword. If an object does not have a name, <code>the target</code> returns its ID. 

The adjectives<code> abbreviated</code>,<code> long</code>, and <code>short</code> return various forms of an object’s name as with the property <code>the name.</code> (Click Related Topics for more information about<code> name</code>.) 

Note: <code>the abbreviated target</code> is the same as<code> the target</code>.

HyperTalk distinguishes between <code>the target</code> and <code>target</code>:<code> the target</code> always returns a string that identifies an object, but the single word <code>target</code> is a container.

 If <code>the target</code> is a button or field, <code>target</code> refers to the contents of that button or field.  If not, <code>target </code>returns an error. 


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

<code><pre>
on whoIsTheTarget
  -- Since the Run the Script button sends a message to the demo script
  -- field, the target is set to it while this handler runs.
  answer "The target is:" && <b>the target</b>
  answer "target (a container) is:" & return & return & ¬
  char 1 to 200 of <b>target </b>-- string must be < 255 chars
end whoIsTheTarget
</pre></code>

## Related Topics

* [name](/HyperTalkReference/properties/name)
* [pass](/HyperTalkReference/keywords/pass)
* [send](/HyperTalkReference/keywords/send)
