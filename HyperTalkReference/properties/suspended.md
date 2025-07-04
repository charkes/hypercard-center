---
title: suspended
card_id: 83697
modified: yes
---

# suspended

`the suspended`

The `suspended` property returns whether HyperCard is currently running in the background under MultiFinder® or under System 7.X. You can switch to another program while a handler is running, and scripts will continue to run in the background.

Use the `suspended` property in a handler to alter the handler’s behavior if it’s running in the background—for example, to avoid displaying `ask` or `answer` dialog boxes.

HyperCard gives time to MultiFinder (and thus to other programs) as follows:

* After it executes each HyperTalk statement in a handler
* Whenever it rotates the busy cursor (during compacting, sorting, and printing)
* During the execution of the `show cards` command and the `wait` command

## Examples

```
if not(the suspended) then
  -- Show a dialog when we're not running in the background:
  ask file "Save as what file?"
  put it into theFileName
else
 --We're in the background, use a default name:
 put "Untitled 1" into theFileName
end if
```

## Related Topics

* [resume](/HyperTalkReference/systemmessages/resume)
* [suspend](/HyperTalkReference/systemmessages/suspend)
* [suspendStack](/HyperTalkReference/systemmessages/suspendStack)
