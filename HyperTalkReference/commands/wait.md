---
title: wait
card_id: 50819
---

# wait

```
wait [for] [ph:posInteger] [ticks]
wait [for] [ph:posInteger] seconds
wait until [ph:trueOrFalse]
wait while [ph:trueOrFalse]
```

The `wait` command causes HyperCard to pause before executing the rest of a handler, either for a specific length of time, until a specified condition becomes true, or while a specified condition remains true.

If you do not specify `seconds` as the unit of time, HyperCard uses ticks. (One tick equals one-sixtieth of a second.)

## Examples

```
wait 7
wait for 7
wait 7 ticks
wait for 7 ticks

wait for 1 second
wait 3 seconds

wait until the mouse is up
wait until the mouseLoc is within the rect of button 1
wait until the sound is done
wait while the commandKey is down
wait while the mouseLoc is within the rect of button 1
wait until the mouseClick
```

## Demo Script

```
on waitUntilTheMouse
  set the cursor to arrow
  show bkgnd field "demo field"
  displayMessage "Click the mouse to continue . . ."
  <b>wait</b> until the mouseClick
  hide bkgnd field "demo field"
end waitUntilTheMouse
```

## Related Topics

* [seconds](/HyperTalkReference/functions/seconds)
* [sound](/HyperTalkReference/functions/sound)
* [ticks](/HyperTalkReference/functions/ticks)
* [time](/HyperTalkReference/functions/time)
