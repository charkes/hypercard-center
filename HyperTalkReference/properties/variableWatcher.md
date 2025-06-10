---
title: variableWatcher
card_id: 87839
modified: yes
---

# variableWatcher

<code><pre>
set [the] variableWatcher ¬
     to <i>resourceName</i>
</pre></code>


The<code> variableWatcher </code>property returns or sets the name of the external command (or XCMD) that displays the Variable Watcher window for inspecting the values of local and  global variables.

The name of HyperCard’s variable watcher is<code> VariableWatcher</code>.

To change the value of a variable using HyperCard’s Variable Watcher, click to select a variable. Its value appears in the bottom panel. Edit the value, and press Enter to save it.

Third-party developers can supply other variable watchers that you can install into HyperCard.

Click Tips for information about the properties of the Variable Watcher.

## Examples

```
set the variableWatcher to "The Inspector" -- if it's installed
```

## Placeholders

[embed:HelpExtras/Placeholders/resourceName.md]

## Related Topics

* [debugger](/HyperTalkReference/properties/debugger)
* [messageWatcher](/HyperTalkReference/properties/messageWatcher)
* [scriptEditor](/HyperTalkReference/properties/scriptEditor)
