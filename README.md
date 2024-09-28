# Radio-Demodulator
![](https://github.com/dagsion/RadioHardware-Demodulator/blob/main/IMG_0835.JPG)

## Introduction
This project entails the collaborative effort of second-year ECE students, tasked with designing subsystems for a Software-Defined Radio (SDR) transceiver. My team, David Xu and Jinyu Xiao, focused on developing the demodulator and audio amplifier, serving as the final link in the receiver chain. This subsystem's core function involves converting processed radio signals into audio and subsequently amplifying it to drive large speakers.

## Design - Single Sideband Demodulator
![](https://github.com/dagsion/RadioHardware-Demodulator/blob/main/Design.png)
This is the design of the SSB demodulator on Altium. It is composed of four stages:
1. Hilbert Transformer creates a 90-degree phase change between the I/Q signal to enable Single-Sideband suppression. It is composed of two-stage all-pass-filters across frequency 100-3200Hz
2. Summing/differential Amplifier is responsible for Single-Sideband suppression.
3. A Negative Power Supply is required for most of the IC chips on the PCB
4. Audio Amplifier which is responsible for producing an audible output from the audio Jack
## Prototype
This is the Altium PCB Design. It is a single-layer double-sided PCB design. The Summing amplifier and the differential amplifier are selected through a switch. The switch also functions as a switch for USB and LSB demodulation. Moreover, the audio amplifier is controlled by a logarithm potentiometer.

![](https://github.com/dagsion/RadioHardware-Demodulator/blob/main/PCB.png)
## Assembly
This is the fully soldered PCB board. These two components left unsoldered which is the design decision we made for the final Low Pass Filter Design. We decide to use a passive Low Pass Filter for simplicity.
![](https://github.com/dagsion/RadioHardware-Demodulator/blob/main/Assembly.JPG)

## Results
Check out this video

https://github.com/dagsion/RadioHardware-Demodulator/assets/117557771/a40ce58c-7ff9-4731-ac77-a94a2d153782

