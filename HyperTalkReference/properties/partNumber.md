---
title: partNumber
card_id: 100450
---

# partNumber

<code><pre>
set [the] partNumber of [ph:part]   ¬
             to <i>integer
</pre></code>

</i>where <code> <i>integer
</pre></code>

</i>is in the range 1 through the  sum of buttons <u>and</u> fields in the current card or background

The <code>partNumber</code> property retrieves or sets the ordinal position of a button or field (that is, of a <u>part</u>) among the total number of all buttons and fields within the same domain (card or background).

Changing a part's <code>partNumber</code> moves it closer to or farther away from the front. 

 For example, the order of buttons and fields on a card is as follows:

button 1  button 2 field 1 field 2 button 3

The <code>partNumber</code> of field 1 is 3. 


## Examples

```

set the partNumber of field 5 to 1 -- farthest back
set the partNumber of cd field Names to number of parts -- closest
get the partNumber of background button "Home"
```

## Related Topics

* [number (property)](/HyperTalkReference/properties/number-property)
