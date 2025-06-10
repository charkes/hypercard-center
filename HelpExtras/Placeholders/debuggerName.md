### debuggerName

The name of the debugger. The HyperTalk debugger is part of the built-in script editor, and its default name is "ScriptEditor." If you add an additional debugger by installing a debugger XCMD, you can choose between ScriptEditor and your new debugger with the HyperTalk command:

<code>set [the] debugger to [ph:debuggerName]</code> or in AppleScript, by setting the <code>debugger</code> property:

<code><pre>
 set debugger to [ph:debuggerName]
</pre></code>
