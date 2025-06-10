---
title: dial
card_id: 34624
---

# dial

<code><pre>
dial [ph:posInteger]
</pre></code>

<code>dial [ph:posInteger] with modem</code> ¬            [[ph:<code>modemCommands</code>] ]<code> </code> The <code>dial</code> command generates touch-tone sounds for the digits in  [ph:<code>posInteger</code>] through the Macintosh speaker. To dial the phone from HyperCard, you must either hold the handset up to the speaker of your Macintosh or use a device that feeds Macintosh audio output to the telephone. 

If you use the <code>with modem</code> option, HyperCard sets up calls using the modem connected to the modem port.  For more information about using modems with HyperCard, see the Phone Dialer stack.  See your modem manual for valid [ph:<code>modemCommands</code>].

Note: If you include a hyphen in the number, place the entire expression in quotation marks. Otherwise, HyperCard performs a subtraction before dialing the number. 


## Examples

```
ask "Enter a phone number:"
if it is not empty then dial it

dial myHomeComputer -- if myHomeComputer contains a number

dial "415-555-1212"  

dial "999-973-6000" with modem  

dial "999-996-1010" with modem "ATS0=0S7=1DT"  -- depends on your modem
```

## Demo Script

<code><pre>
<code><pre>
on mouseUp
 <b>dial</b> "(123) 456-7890"
end mouseUp
</pre></code>
</pre></code>

## Related Topics

* [dialingTime](/HyperTalkReference/properties/dialingTime)
* [dialingVolume](/HyperTalkReference/properties/dialingVolume)
