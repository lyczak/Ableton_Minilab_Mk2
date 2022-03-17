#  Ableton Minilab Mk2 Control Script

This is my personal version of a control script adapted from 
[soneu03/Ableton_Minilab_project](https://github.com/soneu03/Ableton_Minilab_project). While Ableton natively supports the Minilab Mk2 as a control surface, 
this support is pretty limited. This script builds on soneu03's functionality 
to add several more pages of controls to the pads and alter general behavior 
and encoder function.

## Features

Although I've relied on a lot of soneu03's code, I've pretty drastically 
changed some of the behavior of the script so I'll outline each thing it can 
currently do below:

### Cueing Clips in Session View

The first page of pads (1-8) directly correspond to tracks in the session view. 
Pressing one of these pads will trigger the currently highlighted clip from 
that row to start playing. For already playing clips, pressing the pad will 
cause that clip to stop.

### General Purpose Functions 

The second page of pads (9-16) offer some additional functions:

9. Global play/pause
10. Global stop
11. Overdub toggle (session record)
12. Undo
13. Instrument/clip toggle
14. Solo current track (exclusive)
15. Arm current track (exclusive)
16. Play/stop scene

### Muting and Arming Tracks

At any time *regardless of whether on pads 1-8 or 9-16* holding down one of the 
encoder push-buttons will enable a temporary mode where each pad once-again 
corresponds each track. To reiterate, in this mode, pads 1-8 and 9-16 map to 
the same 8 tracks so it doesn't matter which page of pads you're on. Holding 
down encoder 1 allows tracks to be turned on/off while encoder 9 allows tracks 
to be armed/disarmed.

## Installing

First make sure to import and store the `Ableton_Minilab_Mk2_Preset.minilabmk2` preset to the device using the arturia MIDI control center. The rest is the same as any other ableton remote script. Copy the `Ableton_mMinilabMk2` 
directory to appropriate directory. On a mac you'd copy it to 
`/Applications/Ableton Live 11 Lite.app/Contents/App-Resources/MIDI Remote Scripts/`

## Additional Notes

These scripts can get a bit convoluted and messy and this one is no exception. 
I'm doing my best to do things "the right way" but it's going to take a bit of 
work to clean things up (even just removing unnecessary debugging comments) so 
I can't promise that'll happen. Additionally, there is a fair amount of 
functionality added by soneu03 that I have decided not to use and much of this 
has ended up as dead code. I may work those features back into what I have here 
but for now, that code is currently unused.

Also, it's worth noting that due to the changes I've made some of the comments, 
notes, or content from soneu03's version of the project will be out-of-date so 
just be aware of that (I may get around to fixing this but again, no promises).