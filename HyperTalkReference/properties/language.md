---
title: language
card_id: 73795
---

# language

<code> set </code>[<code>the</code>]<code> language to [ph:resourceName]

</code>where <code>[ph:resourceName]</code> is a language supported by HyperCard.

The <code>language</code> property returns or sets the language in which HyperCard displays scripts. The default setting is<code> English</code>, and it’s always available. 

 To use other languages, a script translator resource must exist in the current stack, any stack later in the message-passing order, or in HyperCard itself.

Contrast this property with<code> the scriptingLanguage of [ph:object</code>], which describes an object's scripting system. 


## Examples

```
if the language is not "English" then 
   sort international by field 1
else
   sort by field 1
end if
```

