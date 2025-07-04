### messageList

A comma-separated list of message names that you want sent when the user chooses a menu item in `[ph:menuItemList]`.

Use `empty` to indicate no message in HyperTalk, or `""` to indicate no message in AppleScript.

For example, the menu message list for the first 9 items on the Go menu would be:

```
"go back,go home,help," & ¬
 "go recent,empty," & ¬
  "go first,go prev,go next," & ¬
   "go last"
```
