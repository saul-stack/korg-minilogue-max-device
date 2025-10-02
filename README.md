# Korg Minilogue – Generative, Reactive MIDI Sequencing

![Max4Live Device](/Images/max-device.png)
### Introduction

This project was completed as part of my university module on computer music design, with the goal of creating a software solution to overcome inherent limits of fixed-architecture audio synthesis, exploring the creative potential of introducing generative patterns into the music-making process 
in both live performance and recording settings.

This involved designing a virtual MIDI control surface with Max/MSP to introduce "semi-modular" capabilities to the Korg Minilogue. The finished patch introduces evolving modulation sequences to MIDI control parameters, both random and responsive. 

![Max4Live Device](/Images/max-device2.png)
---

### Signal Flow
![Signal Flow Diagram](/Images/signal-flow.jpg)


### Project goals

#### High-level
- Build a tool to satisfy my own curiosity and provide creative utility to others

#### Design/technical
- Introduce responsive, generative and pseudo-random data streams to extend the capabilities of a fixed architecture synthesizer, with flexibility for other devices in future

#### Learning goals
- Gain fluency in Max/MSP
- Develop knowledge of MIDI communications and standards
- Improve user interface design skills in the context of music technology

## Project justification/inspiration


#### Limitations of the Korg Minilogue

- Limited built-in 16-step sequencer
- Only 2 basic LFOs without phase/trigger controls or complex modulation- only basic waveforms.
- Limited signal routing- no routing matrix
- No random or generative elements

#### Inspiration
- Modular hardware platforms such as Eurorack
- [VCV Rack](https://vcvrack.com/) virtual modular synthesis
- Andrew Norris’ [Minilogue Controller](https://andrewnorris.uk/minilogue-controller/)

### Development Process

#### Research
- Studied the MIDI CC standard
- Installed Max and began practising

#### Planning and presentation

- Determined project bounds and fundamentals
- Presented my proposal to the class and project lead. Received feedback and questions


#### Design

1.	Read, documented and verified Minilogue MIDI CC parameter [addresses](#minilogue-midi-cc-parameters) using Ableton Live 
2. Established two-way communication between Max and the Minilogue and developed functionality
3. Frontend- designed a polished user interface with color themes and audio-reactive sonograph.
4. Compiled the patch as a Max4Live plugin.

## References

#### Docs

- [Max 7 color documentation](https://docs.cycling74.com/legacy/max7/vignettes/max_colors)  
- [Optimisation (change object)](https://docs.cycling74.com/max5/refpages/max-ref/change.html)
- [Demystifying MaxMSP PDF](http://www.paulschuette.com/wp-content/uploads/2013/01/DEMYSTIFYING-MAXMSP.pdf)  
- [Max & Chords PDF](http://peterelsea.com/Maxtuts_basic/Max&Chords.pdf)
- [Max/MSP Patch for Interface Control](https://www.researchgate.net/figure/Max-MSP-Patch-for-the-Interface-Control_fig4_45921721) 

#### Forum Discussions

##### Cycling 74

- [Disable oscillators when receiving no input](https://cycling74.com/forums/how-to-turn-off-a-phasor-when-it-is-no-longer-receiving-data)  
- [Sending a bang on button press](https://cycling74.com/forums/how-can-you-send-1-when-button-flashes-send-0-when-button-turns-off)  
- [Invert a toggle/binary value](https://cycling74.com/forums/basic-question-how-to-invert-toggle)  
- [Editing messages](https://cycling74.com/forums/changing-values-in-a-message-box)  
- [Create LFO and output numerical MIDI values](https://cycling74.com/forums/create-lfo-and-output-numerical-values-create-an-lfo-control-midi-values)  
- [Zen of the Silent Patch LFO Tutorial](https://cycling74.com/tutorials/lfo-tutorial-1-the-zen-of-the-silent-patch/)  
 

##### Reddit

- [Sending periodic bangs](https://www.reddit.com/r/MaxMSP/comments/awir30/advice_on_sending_periodic_bangs/)
-  [LFO that outputs number values](https://www.reddit.com/r/MaxMSP/comments/879hbe/how_do_you_make_an_lfo_that_outputs_a_n) 

#### Articles
- [MIDI to CV conversion](https://loopopmusic.com/midi-to-cv-and-back-can-your-regular-synth-become-semi-modular)
- [Fly-out panel patch](https://web.archive.org/web/20180525153720/https://www.joshuacasper.com/max-4-live-tutorials/fly-out-panel-patch/)

#### Videos
- [JSUI & GUI in JavaScript](https://www.youtube.com/watch?v=1P|U1VyRZ7k)  

#### Minilogue MIDI CC Parameters
![Korg Minilogue MIDI CC](/Images/minilogue-cc-commands.png)