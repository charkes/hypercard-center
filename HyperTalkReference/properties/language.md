---
title: language
card_id: 73795
---

# language

` set `[`the`]<code> language to [ph:resourceName]

</code>where `[ph:resourceName]` is a language supported by HyperCard.

The `language` property returns or sets the language in which HyperCard displays scripts. The default setting is` English`, and it’s always available. 

 To use other languages, a script translator resource must exist in the current stack, any stack later in the message-passing order, or in HyperCard itself.

Contrast this property with` the scriptingLanguage of [ph:object`], which describes an object's scripting system. 


## Examples

```
if the language is not "English" then 
   sort international by field 1
else
   sort by field 1
end if
```

