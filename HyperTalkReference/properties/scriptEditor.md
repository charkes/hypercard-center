---
title: scriptEditor
card_id: 80403
---

# scriptEditor

```
set [the] scriptEditor ¬
    to [ph:resourceName]
```

The `scriptEditor` property returns or sets the name of the current script editor.

The default value of this property is `ScriptEditor`, the name of HyperCard’s built-in editor and debugger.  (The built-in editor and debugger are integrated.)

Because HyperCard’s script editor is actually an [g:external command] (XCMD), you can replace it with your own or third-party script editors.

If HyperCard can’t find a script editor with the specified name, it uses its built-in script editor.

## Related Topics

* [debugger](/HyperTalkReference/properties/debugger)
* [edit script](/HyperTalkReference/commands/edit-script)
* [messageWatcher](/HyperTalkReference/properties/messageWatcher)
* [script](/HyperTalkReference/properties/script)
* [scriptTextSize](/HyperTalkReference/properties/scriptTextSize)
* [scriptTextFont](/HyperTalkReference/properties/scriptTextFont)
* [variableWatcher](/HyperTalkReference/properties/variableWatcher)
* [Set the font and size of a script](/HyperTalkReference/editingscripts/Set-the-font-and-size-of-a-script)
