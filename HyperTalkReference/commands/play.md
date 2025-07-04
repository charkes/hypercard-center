---
title: play
card_id: 43407
modified: yes
---

# play

```
play stop
play [ph:sound]

play [ph:sound] [ph:notes]
play [ph:sound] tempo [ph:posInteger]
play [ph:sound] tempo [ph:posInteger] [ph:notes]
```

The `play` command plays a sound or a series of notes using a sound through the speaker of the Macintosh (or through the audio jack if it’s in use).

`Play stop `stops the current sound immediately; otherwise, the sound plays until it’s done and stops by itself.

<b>Important</b>: HyperCard continues to run handlers and perform other actions while a sound plays. Use the command `wait until the sound is done` to stop a handler until the sound is done playing.

The text string `[ph:notes]` is an unlimited sequence of words in which each word represents one note. A note has the following NAOD format (Name, Accidental, Octave, and Duration):

```
Name        one of these letters:
            a, b, c, d, e, f, g, r
            (where r = rest)
Accidental  one of these characters:
            #, b
Octave      a positive integer
            (4 is middle C)
Duration    one of the letters:
            w, h, q, e, s, t, x
            where
            w = whole note
            h = half note
            q = quarter note
            e = eighth note
            s = 16th note
            t = 32nd note
            x = 64th note
```

You don't have to specify the accidental, octave, or duration of a note. Initially, the accidental defaults to none. The octave and duration default to the <b>same values as the previous note</b>, or to `4` (octave) and `q` (duration) for the first note.

Specify the note r to get a rest. For example: `re --eighth note rest`

A duration followed by a period (.) means a dotted note. A duration followed by the number 3 means one note of a triplet.

HyperCard can also play digitized sounds stored as 'snd ' resources. Use `play` with the name of the resource as the sound. The resource must appear in the current stack, a stack being used, or the Home stack.

HyperCard requires more RAM to play large digitized sounds—about 22K for every second the sound plays.

If HyperCard can't find the sound or load it into memory, `the result` gets `Couldn't load sound`.  If the volume is set to 0, if an XCMD is using the sound channel, or if HyperCard is running in the background, `the result` gets `Sound is off`.

## Examples

```
play "boing"
play "harpsichord"

play "Moo" -- if you have installed this sound into a stack

play "boing" "c e f f# g f e d c"
play "boing" tempo 150 "c e f f# g f e d c"
```

## Related Topics

* [beep](/HyperTalkReference/commands/beep)
* [sound](/HyperTalkReference/functions/sound)
* [wait](/HyperTalkReference/commands/wait)
