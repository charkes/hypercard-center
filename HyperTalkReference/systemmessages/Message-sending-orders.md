---
title: Message sending orders
card_id: 4312
---

# Message sending orders


For some events, HyperCard automatically sends a sequence of system messages.

For example, when you close an existing stack by opening another one, HyperCard sends the following system messages in order: `closeCard`, `closeBackground`, `closeStack`, `openStack`, `openBackground`, `openCard`.

Click an event to see the order in which HyperCard sends multiple system messages in response to it.

### HyperCard startup

When HyperCard first starts up, it sends the following messages in order:

```
startup
openStack
openBackground
openCard
```

(In version 1.2.5, the order was `openStack` `openBackground` `openCard` `startup`.)

### Resume

When HyperCard first resumes after being suspended, it sends the following messages in order:

```
resume
openStack
openBackground
openCard
```

(In version 1.2.5, the order was `openStack` `openBackground` `openCard` `resume`.)

### New stack

When HyperCard creates a new stack, it sends the following messages in order:

```
closeCard closeBackground closeStack
newStack newBackground newCard
openStack openBackground openCard
```

(In version 1.2.5, the order was `closeCard` `closeBackground` `closeStack` `openStack` `openBackground` `openCard` `newStack`.)

### New stack in a new window

When HyperCard creates a new stack in a new window, it sends the following messages in order:

```
suspendStack
newStack
newBackground
newCard
openStack
openBackground
openCard
```

(This event does not occur in version 1.2.5.)

### New background

When HyperCard creates a new background, it sends the following messages in order:

```
closeCard
closeBackground
newBackground
newCard
openBackground
openCard
```

(In version 1.2.5, the order was `closeCard` `closeBackground` `openBackground` `openCard` `newBackground` `newCard`.)

### New card

When HyperCard creates a new card, it sends the following messages in order:

```
closeCard
newCard
openCard
```

(In version 1.2.5, the order was `openCard` `newCard`.)

### Delete stack

When HyperCard deletes a stack, it sends the following messages in order:

```
closeCard
closeBackground
closeStack
deleteStack
```

(In version 1.2.5, the order was `deleteStack` `closeCard` `closeBackground` `closeStack`.)

### Delete background

When HyperCard deletes a background, it sends the following messages in order:

```
closeCard
closeBackground
deleteCard
deleteBackground
```

(In version 1.2.5, the order was `deleteBackground` `deleteCard`.)

### Delete card

When HyperCard deletes a card, it sends the following messages in order:

```
closeCard
[closeBackground]
deleteCard
[deleteBackground]
[openBackground]
openCard
```

The messages in braces are sent only if the deleted card was the last card of a background. (In version 1.2.5, the order was `deleteCard` `closeCard`.)

### Cut card

When HyperCard cuts a card, it sends the following messages in order:

```
closeCard
[closeBackground]
deleteCard
[deleteBackground]
[openBackground]
openCard
```

The messages in braces are sent only if the cut card was the last card of a background. (No messages were sent in version 1.2.5 for this event.)

### Paste card

When HyperCard pastes a card, it sends the following messages in order:

```
closeCard
[closeBackground]
[newBackground]
newCard
[openBackground]
openCard
```

The messages in braces are sent only if the pasted card is the first card of a new background. (In version 1.2.5, the order was `openCard`.)

## Related Topics

* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
