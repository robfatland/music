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
- Modify channel color: shift + click on the track label; also works in the mix console
- Mixer EQ graphic interactive: click on the thumbnail
