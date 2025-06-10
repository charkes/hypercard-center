---
title: version
card_id: 88369
modified: yes
---

# version

<code><pre>
the version [of HyperCard]
the long version [of HyperCard]
the version of <i>stack</i>
</pre></code>


The<code> version </code>property returns the version number of the HyperCard application that is currently running. You can’t<code> set </code>the<code> version</code>.

The<code> long version </code>returns an 8-digit number in the form<code> xxyyzzrr </code>as follows:

* <code>xx </code>: The major revision number
* <code>yy </code>: The minor revision number
* <code>zz </code>: The software state, where
**        80 = final
**        60 = beta
**        40 = alpha
**        20 = development
* <code>rr </code>: The release number

For example,<code> 02206044 </code>is version 2.2 beta release 44, and<code> 02208000 </code>is version 2.2 final.

The<code> version of <i>stack</i> </code>returns a comma-separated list of five numbers in the format of Macintosh version resources:

* Item 1 is the version of HyperCard     that created the stack.

* Item 2 is the version that last     compacted the stack.

* Item 3 is the oldest version to change     the stack since the last Compact Stack.

* Item 4 is the version that has most     recently changed the stack.

* Item 5 is the number of seconds from  12:00 midnight 1/1/04 to the last time     that the stack was changed.

## Examples

```
if item 1 of the version of this stack < "02208000" then ...
```

## Demo Script

<code><pre>
<code><pre>
on answerTheVersion
 answer "The version is:" && the <b>version</b> & return &¬
 "The long version is:" && the <b>long version</b>
end answerTheVersion
</pre></code>
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/stack.md]

