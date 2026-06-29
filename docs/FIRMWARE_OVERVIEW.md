# Firmware Overview

## Target Platform

- Silicon Labs C8051F120
- 8051-compatible high-speed core
- Assembly Language firmware
- Dual-processor architecture
- Deterministic interrupt-driven real-time synthesis

## Main Concept

WELLENKRAFT 8051 distributes the 8-voice synthesis engine over two C8051F120 processors.

Each processor handles four complete voices.  
This allows every voice to retain the full synthesis structure instead of reducing feature depth for higher polyphony.

## Real-Time Responsibilities

The firmware performs:

- DDS oscillator generation,
- wavetable addressing,
- envelope generation,
- digital filter processing,
- MIDI parsing,
- control-change handling,
- program/parameter management,
- communication with external memory,
- control of audio support hardware.

## Effects

The main 8051 firmware does not calculate complex effects such as reverb or chorus.  
Those tasks are handled by a dedicated SPIN FV-1 DSP.  
The 8051 controls program selection and effect parameters.

## Module Differences

Module 1 and Module 2 are structurally similar but not identical.  
Keep both firmware trees separate.
