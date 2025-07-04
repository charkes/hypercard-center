### debuggerName

The name of the debugger. The HyperTalk debugger is part of the built-in script editor, and its default name is "ScriptEditor." If you add an additional debugger by installing a debugger XCMD, you can choose between ScriptEditor and your new debugger with the HyperTalk command:

`set [the] debugger to [ph:debuggerName]` or in AppleScript, by setting the `debugger` property:

```
 set debugger to [ph:debuggerName]
```
