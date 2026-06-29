# Source File Map

## Main Files

| File | Description |
|---|---|
| `wellenkraft.a51` | Main firmware file, interrupt vectors and core synthesis logic |
| `midi.a51` | MIDI implementation and parameter mapping |
| `midi_alt.a51` | Alternative / older MIDI implementation, Module 1 only |
| `init.a51` | C8051F120 initialization |
| `SMBus.a51` | SMBus / I²C communication |
| `PT2257.a51` | Electronic volume controller interface |
| `25VF020.a51` | SPI flash access routines |
| `exRAM.a51` | External RAM support |
| `arduino.a51` | Historical communication interface naming; retained for archive completeness |
| `wheel.a51` | Wheel / performance control routines |
| `Log.a51` | Logarithmic table or mapping support |

## Include Files

| File | Description |
|---|---|
| `f120.inc` | C8051F120 SFR and register definitions |
| `lfo.inc` | LFO tables |
| `phases.inc` | phase / tuning tables |
| `velo.inc` | velocity tables |
| `waves_1.inc` | waveform table data |
| `waves_2.inc` | waveform table data |

## Release Outputs

| File | Description |
|---|---|
| `MODULE1_Modul1.BIN` | Module 1 binary image |
| `MODULE1_PWDS.HEX` | Module 1 Intel HEX output |
| `MODULE2_Modul2.BIN` | Module 2 binary image |
| `MODULE2_PWDS.HEX` | Module 2 Intel HEX output |
