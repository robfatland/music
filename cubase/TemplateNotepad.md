Latest updates to template

To Do
=====
- Time stretch applied to reference track procedure is on github; should have a version here
- Review gain staging
- Describe how this template is configured
- Describe clave rhythm

Importing existing audio
========================
- Get the audio playing on the computer (YouTube, Spotify, etc etc)
- Cubase: Set the Template ref track input to S/PDIF
- Focusrite Clarett+ 4Pre Control app
    - Note the Playback (e.g. 1-2) where the track signal bouncing is apparent
        - The goal is to set this as the S/PDIF Output: Select S/PDIF Outputs, lower left 
        - Ensure S/PDIF Outputs 1-2 has the noted Playback as its input, is not muted
- Cubase: Record the ref track, clean edges, alt-drag copy to the safe reference track
- Bounce both so the events are mutually independent
- Hide the safe ref track (exists in case operations on the reference go awry)
    

Make an instrument from an audio clip
=======================================
- to-do: How to make one pitch serve for all, at any duration?


Gain staging 
============

- todo: Proper links to 'Featherlightstudio' + Dom Sigalas "trick for LOUD mixes" + MixbusTv
- todo: revisit the sources and write these notes coherently
- -12 on Master Bus while Producing / Mixing is the goal
- Loudness is in the Mix (concluding at the Master)
- Let's try and understand "crest factor": Peak to RMS ratio
- Audio tracks
    - Audio natively -12 to -18dB
        - Method 1: Use clip gain event-by-event
        - Method 2: Circle-e channel settings: edit window: Pre-Gain (happens before all downstream processing)
           - Can also get to this on the Mixer
- Dom is all about gain staging before you get into mixing.
    - He drops a loop in a track from Media Bay (drums) + an audio track: clipping. 
    - The problem with dealing with source attenuation with faders: Losing resolution of the fader. 
    - Clip gain: Better than faders; but this turns into micro-visuals on the waveforms.
    - Pre-gain: Fader is where it wants to be (at 0) and the waveform is not crushed.
    - Event-based volume editing: Pencil tool, tick dots along the upper edge of the event and drag them down to moderate the audio waveform.
    - *Then* the clip gain event volume handle up/down comes in.
    - *Then* fader: Enable Write automation.
- MIDI tracks
- Plugin-to-Plugin
    - Example 1176 Compressor emulator sees a level that can be affected by the EQ
        - So changing the EQ changes compression in addition to changing the sound of the track
    - Use the in/out toggle to check
    - Do not let 'louder is better' control the process
- Digital / Analog back out into the world
    - Leaving the DAI: Look at the Audio Connections: control for output gain control
- Busses / Masters
    - Clipping with a lot of groups and busses coming in is a common issue
        - Turn the Master bus down so it does not clip
        - At the same time we want the signal to the monitors sounding good. Whatever that means. 
        - So not clipping the Master bus is the name of the game: Peak metering
            - RHS of the DAW
            - Main meter: RMS and Peak value 
            - Other tab: LUFS and other features
            - LUFS is overall loudness overtime... something like -14 is a good LUFS level
            - True Peak should be well below Zero




==== Create an instrument from a sound clip

Gain staging from 'Featherlightstudio' + Dom Sigalas "trick for LOUD mixes" +
MixbusTv

>     -12 on Master Bus while Producing / Mixing is the goal
>     The Loudness is in the Mix (concluding at the Master)
>     Let's try and understand "crest factor": Peak to RMS ratio


Part 1: Audio tracks
    - Audio natively -12 to -18dB
        - Method 1: Use clip gain event-by-event
        - Method 2: Circle-e channel settings: edit window: Pre-Gain (happens before all downstream processing)
           - Can also get to this on the Mixer

Dom is all about gain staging before you get into mixing.
He drops a loop in a track from Media Bay (drums) + an audio track: clipping. 
The problem with dealing with source attenuation with faders: Losing resolution of the fader. 
Clip gain: Better than faders; but this turns into micro-visuals on the waveforms.
Pre-gain: Fader is where it wants to be (at 0) and the waveform is not crushed.
Event-based volume editing: Pencil tool, tick dots along the upper edge of the event and drag them down to moderate the audio waveform.
*Then* the clip gain event volume handle up/down comes in.
*Then* fader: Enable Write automation.




Part 1B: MIDI tracks


Part 2: Plugin-to-Plugin
    - Example 1176 Compressor emulator sees a level that can be affected by the EQ
        - So changing the EQ changes compression in addition to changing the sound of the track
    - Use the in/out toggle to check
    - Do not let 'louder is better' control the process


Part 3: Digital / Analog back out into the world
    - Leaving the DAI: Look at the Audio Connections: control for output gain control


Part 4: Busses / Masters
    - Clipping with a lot of groups and busses coming in is a common issue
        - Turn the Master bus down so it does not clip
        - At the same time we want the signal to the monitors sounding good. Whatever that means. 
        - So not clipping the Master bus is the name of the game: Peak metering
            - RHS of the DAW
            - Main meter: RMS and Peak value 
            - Other tab: LUFS and other features
            - LUFS is overall loudness overtime... something like -14 is a good LUFS level
            - True Peak should be well below Zero

