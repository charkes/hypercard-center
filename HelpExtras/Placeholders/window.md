### window

One of HyperCard’s built-in windows, the window containing the current stack (called the card window), or any other window containing a stack, as follows:

<code><pre>
card window
tool window
window "tools"
pattern window
window "Patterns"
scroll window
window "scroll"
[the] message [window]
[the] message [box]
[the] msg [window]
[the] msg [box]
window "message"
message watcher
window "message watcher"
variable watcher
window "variable watcher"
window "Home"
window "Readymade Buttons"
-- if longWindowTitles is true:
window "My HD:Home"
window 6
window ID 21403082
</pre></code>

Note: If a window containing a stack is inactive, you can set only its <code>location</code> and <code>visible</code> properties.

<b>Important</b>: External windows can’t be substituted for the <code>[ph:window]</code> placeholder (see the <code>[ph:externalWindow]</code> placeHolder).
