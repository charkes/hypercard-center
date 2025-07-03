---
title: systemVersion
card_id: 102613
---

# systemVersion

```
the systemVersion
```

Value returned: a decimal string representing the running version of system software

Use this function, for example, to determine if a particular command or handler will run correctly under the current version of the system software.

## Examples

```
if the systemVersion < 7
then answer "AppleEvents not available under this system"

put the systemVersion
```
