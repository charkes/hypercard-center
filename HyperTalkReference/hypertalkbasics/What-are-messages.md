---
title: What are messages?
card_id: 5306
modified: yes
---

# What are messages?

A message is simply an announcement that an event has occurred: The user has clicked the mouse, requested the answer to `4 * 3`, added a new card to a stack, and so on.

To understand messages, think of mailing a letter to a friend. You write a message and place it inside an envelope. Then you address the envelope and send it to your friend.

HyperCard does the same thing:

1. It determines the content of a message (what just happened).
2. It decides where to send the message.

### What’s the content of a message?

The message itself is just HyperCard’s name for the event that occurred. HyperCard acts as a translator: it “watches” the stack and translates events into message names.

To see HyperCard translate events into message names, move the pointer over the Example Button and click.

### Where does HyperCard send the message?

HyperCard determines what object the user has acted on and uses this as the “address” for the message. HyperCard then sends the message to one of its objects:

* a button
* a field
* a card
* a background
* a stack

Once HyperCard knows both the content of the message (the message name) and the destination of the message (where to send it), it sends the message to the object.

## Related Topics

* [Handling messages](/HyperTalkReference/hypertalkbasics/Handling-messages)
* [on](/HyperTalkReference/keywords/on)
* [Writing function handlers](/HyperTalkReference/hypertalkbasics/Writing-function-handlers)
* [Writing message handlers](/HyperTalkReference/hypertalkbasics/Writing-message-handlers)
