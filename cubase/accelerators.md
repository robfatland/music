# accelerators

Tips-N-Tricks YouTube playlist transcribed here into a cheat sheet.


General rule of thumb: There are so many menus / items so it may help to scan menus. Example: Not 
finding it in Edit > Key Commands? Maybe check Transport.


## en passant


- Grid type: Adapt to zoom
- Multi-track selection: Hold shift + ctrl + range selection tool drag
- Loop on range selection: alt-p (event select or range selection tool)


## [Dom Sigalas workflow shortcuts](https://www.youtube.com/watch?v=C67OjuSL90U)


- Chopping to quantize value: Scissors > Alt + Click
    - Set quantize to 16 notes with snap activated 
- J toggles snap on and off
- Zoom in and zoom out
    - h and g: So far so good
    - alt-g/h zooms vertically
    - shift-g/h zooms waveforms in tracks
- editing an audio track (say vocal): Want to lower level on a breath
    - deactivate snap, range selection tool, shift + x, lower that signal
- Customize feature: open quantize panel: ctrl + alt + q
    - Create a shortcut
- Reset quantize for selected MIDI notes: ctrl + shift + q
    - Create a shortcut: How?
        - Edit > key commands > search on 'reset quant' to find; enter key combo, click assign
- Add track: instrument: ctrl + alt + n, audio: ctrl + alt + m 
- Select an event + p to move the cycle markers to bracket the event
- Quantize increase/decrease: \[ and \] keys
    - Edit > key commands > select next / previous quantize
- Cycle through snap types: ctrl + \[ and \]
    - Select previous / next snap type


## [More Dom Sigalas tips n trix](https://youtu.be/boyPW1TNWvU?si=DRcnRWoInolWSpSD)


- Range selection tool: Selection palette: Far left: Combine with selection (cursor) tool
    - RST at the upper half of an event / ST at the lower half!
    - Things to do:
        - Select a range, then shift-X to turn that into an event (rather than clipping both sides)
        - Select a range, then alt-drag it
        - Of course alt-D to duplicate many times
        - Range select and then delete to clean up a track
- J disable / enable snap
    - While doing a range select: Hit ctrl to disable snap in that select
- Faster and more precise **fade outs**
    - select the parts of the tracks where you want it, then **a** (same for fade-in)
- **Global Copy** to make space in the interior of the track for some inserted music
    - Set Locators
    - Edit > Range > Global Copy
    - Move the cursor to where it is to be **inserted**
    - Edit > Range > Paste Time: Boom!
- Chop / Stutter Effects with the scissors
    - Select an event and then select the cut / scissors tool
    - alt + click on quarter note (say) to split the event on quarter notes; or 8th, 16th
    - switch to the mute tool and mute certain (now micro) events
    - or look in Key Commands for the alias for mute / unmute objects; Dom uses the v key
- Assigning key commands
    - Examples: Silence (shift + space) and Reverse (ctrl + alt + R)
- One track: Multiple consecutive events
    - Select events
    - Audio > Events to Part (shortcut shift + D)
    - A part is indicated by a meta-box (logical container) with the events inside like boxcars
    - Can edit; can reverse with 'Dissolve part'
- Zooming
    - Select a focus event > alt + S zooms to this event
    - Alias alt + z to unzoom
    - See the Edit > Zoom menu
    - Zoom out to project scale: shift + F
- Edit cut head + tail (respective crap at start/end of an event)
    - select event, cursor locate, alt + \[ for head, alt + \] for tail
    - (see Key Commands cut head / cut tail)
- Offline process **Presets**
    - Say you commonly want to "add chorus delay + reverb to audio events" or some such common task
    - Audio > Direct Offline Processing > + Plug-in, drag it into the Favorites box
    - Have that box up; select an event; apply it by clicking the process


## [Dom Sigalas MIDI tips](https://youtu.be/hYkjXVW1NTA?si=2yFb92GAiozh64TT)


- To do


 ## [Chris Selim tipsntrix](https://www.youtube.com/watch?v=YfrXbaOa4Uc&list=PLBxAzSicPZqRhiwalnHbmYMAiB1gP8Djm)


 - Duplicate an audio track with the new version pre-bounced / decoupled from the source
    - This will create an independent audio file superseding "everyone points to the same file"
    - I did this: Edit > Preferences > Editing > Audio > On Processing Shared Clips > Open Options Dialog
    - Test it by doing some VariAudio on the new track
- Rename an audio event
    - Select an event; info line top of screen: under Description: Rename
    - Note text in paren on the event is the name of the source audio file
- Ripple delete (auto-collapse) snap right events to left-most event after a delete operation
    - In Cubase this is called Delete Time
    - Range selection tool: select
    - Shift + backspace
    - Edit > Range > Delete time
    - Let's do this on the full project: The select process is shift + control + range select; then shift + backspace
- Create my own VST Instrument list
    - Studio > VST Plugin Manager
- Mixer fader items
    - Faders up to 12dB: Project > Set up > Fader max
    - Fader micro moves: Hold down shift: Now fader moves are very small
- Modify channel color: shift + click **LEFT SIDE** of track name panel (i.e. in the color); also works in mix console
- Mixer EQ graphic interactive: click on the thumbnail
