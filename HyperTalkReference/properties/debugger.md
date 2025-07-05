---
title: debugger
card_id: 92176
---

# debugger

```
set [the] debugger to debuggerName
```

The debugger property returns or sets  the name of the current HyperTalk debugger. The default value of this property is `ScriptEditor`, the name of HyperCard’s built-in editor and debugger. (The built-in editor and debugger are integrated.)

Click Related Topics for more information about debugging a script.

Because HyperCard’s debugger is actually an [g:external command] (XCMD), you can replace it with your own or third-party debuggers.

If HyperCard can’t find a debugger with the name provided, it uses its built-in debugger.

## Related Topics

* [debug](/HyperTalkReference/commands/debug)
* [Debug a script](/HyperTalkReference/editingscripts/Debug-a-script)
* [messageWatcher](/HyperTalkReference/properties/messageWatcher)
* [scriptEditor](/HyperTalkReference/properties/scriptEditor)
* [variableWatcher](/HyperTalkReference/properties/variableWatcher)
