---
title: scriptingLanguage
card_id: 100648
---

# scriptingLanguage

 <code>set [the] scriptingLanguage ¬      [of [ph:object ]] to <i>languageName

</code></i>where [ph:`languageName`]  is HyperTalk or the name of any OSA-compliant  scripting system such as AppleScript.

The `scriptingLanguage` property sets or retrieves  the scripting system of the object or (when you don't use ` of [ph:object] `) of the message box. 

[ph:`LanguageName `]must be present in the computer's system resources. 

 The message box and each individual object can all respond to different scripting systems.

You can also set the `scriptingLanguage` property for an object by choosing from the Scripting Language pop-up menu at the top of each object's script editor window.

The default [ph:`languageName`]  is HyperTalk. 


## Examples

```


get the scriptingLanguage of bg button 6

set the scriptingLanguage to AppleScript -- for Message box only
```

## Related Topics

* [Debug a script](/HyperTalkReference/editingscripts/Debug-a-script)
* [debugger](/HyperTalkReference/properties/debugger)
* [edit script](/HyperTalkReference/commands/edit-script)
* [HyperTalk and scripts](/HyperTalkReference/hypertalkbasics/HyperTalk-and-scripts)
* [messageWatcher](/HyperTalkReference/properties/messageWatcher)
* [Open a script window](/HyperTalkReference/editingscripts/Open-a-script-window)
* [Save a script](/HyperTalkReference/editingscripts/Save-a-script)
* [script](/HyperTalkReference/properties/script)
* [scriptEditor](/HyperTalkReference/properties/scriptEditor)
* [variableWatcher](/HyperTalkReference/properties/variableWatcher)
