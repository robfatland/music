# Cubase


- I start new Cubase projects from my standard template. This has a notepad plain text file built in with some 
notes; so the master is in this folder as `TemplateNotepad.md`.
- For more involved notes I'll create other material in this Cubase subfolder
- The rest of this file as of Dec 2024 is miscellany
  

## YouTube resources

- [One Man And His Songs](https://www.youtube.com/@OneManAndHisSongs) Antony is the person for methodical, thorough, relatable Cubase and Halion skills
    - [Halion 7 series](https://www.youtube.com/watch?v=3FXFOoMp6Jw&list=PL3P42Av427hwDrDjdiGnIdA_qAiWJDrkI)
- [Dom](https://www.youtube.com/@DomSigalas) our guy
- [MartynHeyne](https://www.youtube.com/@martynheynemusic) is a pro producer with excellent art of production content 
- [VST Instruments and Plug-Ins](https://www.youtube.com/@VSTInstrumentsPlugIns) includes Dom Sigalas, seems current, lots of content many topics
- [Steinberg](https://www.youtube.com/@steinberg)
- [MusicRadar Tech](https://www.youtube.com/@MusicRadarTech)
- [ADSR Pro](https://www.youtube.com/@MikeSmithADSRPro) is antiquated content still relevant: synth sound building; check out vocal chopping


## Terms 


- CC is Continuous Controller for MIDI and it means something like a pitch bend wheel that can emit a string of modifiers.
- Two loudness acronyms: Loudness, K-weighted, relative to full scale (LKFS) or Loudness Units (LUFS)


## Pre or Post Fader?

As a rule: Effects sends follow the fader ("post fader", Cubase control is orange) 
so that whatever the effect is doing stays in relation to the signal from
the source. When might the send be switched to pre-fader (blue)? 
The way to think about this is imagining starting with the fader at Zero and putting the effect in front of the fader; 
then dropping the fader and seeing the "ghost" result taking over for the main signal. Maybe side-chaining
compression would be a candidate where you fade down a kick but still use it to trigger the compressor.


## Gain Staging


From Dom Sigalas (and others)


The goal is -12 dB on the master bus, leaving headroom in the mix. Initial gain stage target is -18dB via PreGain 
as a rule of thumb.
Drums cut through hotter; so pushing them to lower, even -24dB, is reasonable. 
The idea (Dom Sigalas, others) is to keep the fader at zero and use other mechanisms to 
get into the ballpark. Then the fader comes in as the last adjustment.

Media Bay loops i.e. pre-built content are by nature VERY HOT. Why? Because it is a Loud World and they have to compete for your attention.

So after the source is connected: Go to the channel strip in the mixer or 
the EQ control for the track, enable PreGain and drag it down into the -18dB ballpark.
Here is a gain staging sequence:


* PreGain to -18dB
* Audio tracks: Use the pencil tool to introduce localized attenuation of hot sections: 'Much more natural sounding than a compressor'
* Audio tracks are Events or Clips; which have clip gain setting (starting at unity): Magnitude of the waveform. Use if necessary.
* Write automation: Using the fader write an envelope during playback. Attention, post: *All* the adjustable stuff, like tilt
* Not covered yet: Full work flow, EQ particularly bass, Compression, Mastering, Mix Down, returning to a loud mix if so desired.


Another pass at this: 
- Loudness is in the Mix (concluding at the Master)
- "Crest factor" is Peak to RMS ratio


Part 1: Audio tracks
    - Audio native -12 to -18dB
        - Method 1: Use clip gain event-by-event
        - Method 2: Circle-e channel settings: edit window: Pre-Gain (happens before all downstream processing)
           - Can also get to this on the Mixer
- Gain staging before mixing
- Audio tracks: Natively -12 to -18 in this order of methods:
    - Pre-gain: Fader is where it wants to be (at 0) optimal pixels for fine-tuning
    - Event-based volume editing: Pencil tool, tick dots along the upper edge of the event, drag down to moderate
    - Event or clip gain 
    - Fader: Enable Write automation.

What about MIDI tracks?


Topic: Plugin-to-Plugin
    - Example 1176 Compressor emulator sees a level that can be affected by the EQ
        - So changing the EQ changes compression in addition to changing the sound of the track
    - Use the in/out toggle to check
    - Do not let 'louder is better' control the process


Topic: Digital / Analog back out into the world
    - Leaving the DAI: Look at the Audio Connections: control for output gain control


Topic: Busses / Masters
    - Clipping with a lot of groups and busses coming in is a common issue
        - Turn the Master bus down so it does not clip
        - At the same time we want the signal to the monitors sounding good. Whatever that means. 
        - So not clipping the Master bus is the name of the game: Peak metering
            - RHS of the DAW
            - Main meter: RMS and Peak value 
            - Other tab: LUFS and other features
            - LUFS is overall loudness overtime... something like -14 is a good LUFS level
            - True Peak should be well below Zero





## Scoring

The best approach I've found to date is to build a MIDI track that is intended for a score. MIDI is easy to edit and quantify. 
The MIDI feeds the Score editor, so printed music. Then mute the MIDI track and record it from a real instrument.


A more circuitous idea that works on an audio track: Use VariAudio to create something that looks like MIDI, then see above.
I haven't done this but it seems like an interesting idea... maybe runs into a brick wall with any polyphony.


Sometimes we start from a keyboard part and want to decompose that into a bassline and a guitar part. I find it helpful to
duplicate the keyboard and treat the lower copy as the proto-bassline. Delete everything except the lowest note and change
the VST Instrument. Then on the upper track do the converse.


The Cubase Score Editor is a learning curve proposition. Do the learning curve before trying to create a score for a project. 
This is painful because it feels slow.


## Side-chaining


## Reverb and Compression


## Tips from Sohn and Chris

- Mixer: Shift + Alt highlights QLink button when activated does everything across multiple selected tracks
- File > Key Commands > L for Locate Selection Start on the Transport and : for Right; use with copy-paste
- Marker track: Can enable toggle between time-based and music-based modes
- Event name change: Select and modify at the top of the Inspector
- Bounce range: Don't just select the Event or Events to bounce: Select a *range* that contains these Events and then Bounce
    - Useful for making tracks start at 1 which facilitates sharing across DAWs
- Backup Project File rather than Save As: Don't use Save As
- Increase the number of automation points in a manual drawing
    - Project > Automation Panel (F6) > Settings > Reduction Level bring down to 5% (less interpolation: more points)
- Channel settings window
    - Change EQ colors: Preferences > MixConsole Rack Colors > Equalizers, PreGain
    - Knob version of EQ: Use dropdown in upper right of the Equalizer tab
    - Can do metering color changes here also: Like -18dB for gain staging purposes
- Mix console: Drag an effect using Alt + Drag; or Drag INSERTS to do all of them; and SENDS; Channel strip; EQ
    - Even drag and drop the entire channel

## Control Room 
- Mixer L button: CR right tab, Main tab, Listen: AFL selected, LE activated, level at 0.0, Listen Dim to hear the mix at a lower level
    - Listen to an effect without the dry signal 

## Keyboard Editor for MIDI

- There is a chord editor built in
- Hold Ctrl to select all notes of a given pitch
    - Also drag a note up/down: Start, THEN hold Ctrl when dragging to lock its time position
        - This works on an Alt copy of a note as well
    - Select note + Ctrl + Shift: Now you are dragging velocity
- Quantize: Lengths, Ends, Reset
- Velocity has three handles: Center global and ends tilt; and side-center is a compressor
    - These controls also work for recorded Modulation
- Modulation: Select + Delete gives back a square wave but with a handle
- > MIDI > Functions
    - Explore!
- Look into the Key Quantizer: Contrains MIDI notes to lie within some key; drag up and down to restructure harmony


## Drums


Dom says four ways: Keyboard drumming (separate video!), Drum Editor, MIDI Insert Beat Designer and Groove Agent Patterns


- Use the keyboard... ok... and double click in the Track Editor to create notes (faster than switching to pencil)
    - Edit volume etc etc
    - Ghost notes very quiet at 1/32 three in a row before a downbeat: nice touch 
- Lower zone > Editor > Dropdown: Drum Editor is open for business
    - Go to the top-center zone > drum track > drag pencil > empty Event (say four measures)
    - Drum editor: Create drum map from instrument
    - Drum editor: Blank column on the left of the Pitch/Instrument table: Click to audition
    - Drum editor: controls bar: left side "home plate" icon with dropdown: Show drum sounds in use by Instrument
        - Later: After instruments are chosen: Show Drum Sounds With Events cleans things up further
    - Why does Dom get diamonds when I get boxes? Why is one version of my kick pathological, the other works?
    - Scale velocities ensemble by selecting notes; then hover in velocity window to see this option
    - Notice velocities are isolated to the selected drum sound; not *everything*
    - When the Drum Editor is engaged the Inspector changes to emphasize Quantize: Can modify / apply to a selected drum
- With a GASE track open Beat Designer from the Track Inspector > MIDI Inserts > Dropdown > Beat Designer
    - Match some segment of the track to the duration of the Beat Designer
    - Velocity, flams, two swing modes, other features
    - Use the upper left dropdown to print patterns onto the track; or better: Drag the desired pattern from the stylized keyboard
        - That stylized keyboard is at the bottom of the BD interface; and notice it has capacity for many patterns
    - Notice there are presets as well
    - There are a limited number of instruments; click on one to see the full available list
- From GASE 


## Project Directory

* Cubase
    * Boom
        * **A Better Place Projects** (November 2014: two sub-folders)
            * A Better Place Produced Multitrack: Boom double-tracked. Includes Rob harmony, keyboard accomp
                * Included mp3 mixdown in **tunes**
            * A Better Place Boom Vocal Source Only
        * Adore
        * Assignment June 2020
        * Boomclavier
        * **Halfway Down Pre-Vocals G+B**: Excellent sound, Takamine + Yamaha + ooooohs
        * Krondar
        * Waiting
    * Covers
    * * Five O O D P F
        * CB 001 Basics
        * HowLongBlues
        * Jazz Drum Track
        * Mom
        * Soul Kitchen surface
    * Rob
        * **Carole** (not everyone survives) ~2000: Four short "Two/Setzer"-related pno segments with ++ good flute in one of them (mp3 upload)
        * **CasinoRoyale Lukagruv** (mp3) is an interesting trombone voice solo over the usual chord progression
        * Criquet
        * Dear Brutus
        * Desert en passant
        * Divertimento
        * Doxology
        * Festes Waltz
        * HappyBirthday
        * Hunt Blues
        * Lukaboom
        * Ooompah Tune
        * **Tempest** (mp3): EDM-style with lyrics from the play; Moog, chorus, pno, funk drums and guitar
        * **Thanks Chuck** (mp3): Fragment of a horn playing over a reverby electric piano, one phrase
        * **Thor Tapped Keef** (mp3): With explanatory Notepad content
            * Keef is a pretty enjoyable fragment; MIDI + Kurz audio remix (needs some production)
        * **Ur-Waiting** (mp3) Most of the ideas of the tune 'Waiting' (see Boom) segues into the F-7 hanging chord riff. MIDI + Kurz Setup
    * Shuvalov: That dreadful tune about frosting (but the groove isn't bad in fact; and it has a rubato middle section)
    * Student
        * Bass
        * Drums
            * **Building Drum Beats** is drum learning curve work
                * Includes beat tracks: Walk This Way, Clave, various Afro-Cuban; sadly mostly empty placeholders
            * Various 808: audition tracks, Shekere track, one drum per track towards groove
        * Guitar
        * Music Production
    * Styles
        * AfroCuban
        * Blues
            * Blues: Short blues/rock (mp3 added); distorted guitar 335 and trumpet; DRUM TRACK is cut and paste, super instructive tho
        * Flamenco
        * Reggae
            * Reggae
* Cubase New
    * Desert (Aug 2021): 'Father ... beer'
    * Stronzi: Simple oom pah groove experiments using a B3 as bass; so interesting bassline
* Cubase T DMAF H
    * DoMeAFavor (July 2021)
        * Mix sounds muffled as if through cotton, 'overproduced'?
        * Notes
            * HALION learning curve: See Halion.md
            * Production notes  
        * Lots of tracking: Guitar and bass. Drums pretty perfunctory. 
