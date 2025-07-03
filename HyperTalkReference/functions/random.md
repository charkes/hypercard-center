---
title: random
card_id: 61729
---

# random

```
the random of [ph:posInteger]
```

Value returned: a random integer between 1 and `[ph:posInteger]`

`Random` returns values for integers up to `2^31 - 2`. 

## Demo Script

```
on hyperMath
  -- This is a very simple math flash card script.
  put <b>random</b>(50) into intOne
  put <b>random</b>(50) into intTwo
  put item <b>random</b>(2) of "+,-" into theOperator
  put intOne && theOperator && intTwo && "=" && ¬
  (the value of (intOne && theOperator && intTwo)) into theAnswer
  put 0 into theCount
  ask "What is" && intOne && theOperator && intTwo
  if it is empty then exit hyperMath
  if it is last word of theAnswer then put "That's right!" & ¬
  return before theAnswer
  answer theAnswer
end hyperMath
```
