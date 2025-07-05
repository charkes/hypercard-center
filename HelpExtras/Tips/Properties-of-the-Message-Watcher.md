---
title: Properties of the Message Watcher
card_id: 53830
---

### Properties of the Message Watcher

By default, the Message Watcher shows only those messages that your scripts actually handle. You can change what the Message Watcher shows using the following properties:

```
the hideUnused of window ¬
   "message watcher"
set the hideUnused of window ¬
   "message watcher" to [ph:trueOrFalse]
```

returns or sets whether the Message Watcher shows all messages, other than idle, that HyperCard sends or just the ones handled by scripts. If set to false, unused messages appear in parentheses.

```
the hideIdle of ¬
   window "message watcher"
set the hideIdle of window ¬
   "message watcher" to [ph:trueOrFalse]
```

returns or sets whether the Message Watcher shows the idle messages that HyperCard sends continuously.

```
set the nextLine of window ¬
   "message watcher" to [ph:text] & return
```

indents the proper number of spaces and adds a line to the Message Watcher. (You can’t get this property.)
