---
title: sum
card_id: 102760
---

# sum

<code><pre>
sum([ph:numberList])
</pre></code>

Value returned:  the sum of a comma- delimited list of items


[ph:<code>numberList </code>]evaluates to  a comma-delimited list of items, including any container holding such a list. 


## Examples

```


put sum(field 5) into total

if sum(firstList) > sum(secondList) then answer "Imbalance Found"
```

## Demo Script

<code><pre>
on mouseUp
  answer "1 + 2 + 3 + 4 + 5 + 6 + 7 =" && <b>sum</b>(1,2,3,four,5,6,7)
end mouseUp
</pre></code>

