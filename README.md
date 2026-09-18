![StepperTune Professional](images/skin.png)

# StepperTune Professional

**Turn MIDI music into G-code and let your Bambu Lab printer play it using its stepper motors.**

StepperTune Professional is a Windows application designed to import, arrange, preview and convert MIDI music into printer-specific G-code for supported Bambu Lab printers.

Originally developed as a simple MIDI-to-G-code converter, StepperTune has evolved into a multi-voice music environment with independent voice control, PC preview, automatic balancing and polyphonic stepper playback on supported printer architectures.

---

## Main Features

### 🎹 MIDI Import

- Load standard MIDI files
- Select MIDI tracks for each voice
- Automatically convert MIDI notes and timing
- Adjust BPM
- Prepare musical arrangements specifically for stepper-motor playback

### 🎼 Up to 3 Independent Voices

StepperTune Professional can manage up to three independent musical voices.

Each voice provides:

- Independent MIDI track selection
- Individual Play / Stop control
- Individual volume control
- Separate musical data
- Independent enable/disable state

The number of available voices automatically adapts to the selected printer.

### 🔊 Monophonic and Polyphonic Playback

StepperTune automatically configures the music engine according to the selected printer architecture.

**Monophonic mode**

- Single musical voice
- Designed for printers using the Cartesian sound driver
- Simplified controls for single-voice playback

**Polyphonic mode**

- Up to three simultaneous voices
- Independent volume for each voice
- Multi-voice PC preview
- Polyphonic G-code generation

This makes it possible to arrange different parts of a MIDI composition and reproduce them simultaneously using the printer's stepper motors.

### ▶ PC Preview

Listen to the arrangement before generating the final G-code.

- Play / Stop individual voices
- Play multiple voices together
- Play All control
- Individual voice volume
- Preview the complete musical arrangement directly on the PC

### ⚖ Auto Balance

StepperTune Professional includes an automatic balancing function for multi-voice arrangements.

Auto Balance helps normalize the relative level of the selected voices before generating the final result.

Manual volume adjustment remains available for each voice.

### 🧩 Printer-Specific G-code Generation

StepperTune automatically selects the appropriate sound driver for the chosen printer.

- Printer-specific G-code generation
- Monophonic or polyphonic output depending on printer architecture
- No manual editing of individual `M1006` notes required for normal use
- Generated music can be used in Start G-code or End G-code
- G-code can be exported ready for use

### 💾 StepperTune Project Files

Projects can be saved in the StepperTune `.stf` format and reopened later.

Project files preserve the main arrangement settings, including:

- Selected printer
- BPM
- Voice configuration
- Voice levels
- Polyphony settings

This allows a composition to be edited later without rebuilding the project from the original MIDI file.

### 🔄 Update Check

- Automatic update check at application startup
- Manual update check from the Help menu
- Online version information

### 📘 User Manual

Italian and English documentation is available for StepperTune Professional.

The manuals cover:

- Interface and controls
- MIDI import
- Voice configuration
- Preview and balancing
- G-code generation
- Bambu Studio integration
- Supported printers
- Safety and usage notes

---

## Supported Printers

| Printer | Playback Mode | Voices |
|---|---|---:|
| Bambu Lab A1 | Monophonic | 1 |
| Bambu Lab A1 mini | Monophonic | 1 |
| Bambu Lab A2L | Polyphonic | Up to 3 |
| Bambu Lab H2D | Polyphonic | Up to 3 |
| Bambu Lab H2S | Polyphonic | Up to 3 |
| Bambu Lab P2S | Polyphonic | Up to 3 |
| Bambu Lab X2D | Polyphonic | Up to 3 |

> Always select the correct printer model before generating G-code.

Printer support refers to the playback mode implemented by StepperTune Professional. Actual behavior may also depend on printer firmware and G-code support.

---

## Tested Printers

The following configurations have been physically tested during development:

- **Bambu Lab A1 / A1 mini** — monophonic playback
- **Bambu Lab H2S / X2D** — polyphonic playback

Additional supported models use the corresponding StepperTune printer architecture and may be validated progressively.

---

## Basic Workflow

1. Select the Bambu Lab printer
2. Import a MIDI file
3. Configure the desired musical voices
4. Select the MIDI track for each voice
5. Set or verify the BPM
6. Preview individual voices
7. Preview the complete arrangement
8. Adjust voice levels or use Auto Balance
9. Generate the printer-specific G-code
10. Export the finished result

---

## Using the Generated Music

StepperTune can generate music for use with the printer's G-code configuration.

The generated sequence can be used as part of the printer's Start G-code or End G-code.

### Bambu Studio

1. Open **Bambu Studio**
2. In the **Prepare** tab, select the correct printer and nozzle size
3. Click **Edit preset**
4. Enable **Advanced**
5. Open the **Machine G-code** tab
6. Locate the existing printer sound section
7. Replace only the sound block with the code generated by StepperTune
8. Preserve the original G-code outside the sound section
9. Save the printer preset

### Important

Do **not** replace the complete Machine start G-code or Machine end G-code.

Only replace the section dedicated to printer sound.

Preserve all G-code line breaks when copying and pasting.

Official Bambu Lab MIDI/G-code reference:

https://wiki.bambulab.com/en/A1-mini/Midi

---

## From StepperTune to StepperTune Professional

StepperTune started as a simple application for creating melodies and converting MIDI tracks into G-code jingles.

The Professional version expands the original concept with:

- Multi-voice arrangements
- Up to three independent voices
- Monophonic and polyphonic printer modes
- Individual voice preview
- Individual voice volume
- Play All
- Auto Balance
- Printer-specific music engines
- StepperTune project files
- Extended MIDI workflow

Previous versions remain part of the project history, while **StepperTune Professional is the current version**.

---

## System Requirements

- Windows
- Bambu Studio
- Supported Bambu Lab printer

---

## Free Activation

StepperTune Professional requires an activation code.

**The activation code is completely free.**

The activation system was introduced to help protect the project and prevent unauthorized commercial redistribution. It is not a paid licensing system and there is no charge for using StepperTune Professional.

Activation codes are provided manually by DGVeLab and are therefore **not generated automatically or immediately**.

After submitting an activation request, please allow some time for a response. Requests are normally processed **within the same day**.

> **StepperTune Professional is free to use.**  
> The activation system exists only to protect the project and its distribution.

---

## Disclaimer

StepperTune Professional is an independent project and is not an official Bambu Lab product.

It is not affiliated with, sponsored by, or endorsed by Bambu Lab.

The application generates G-code commands that operate printer motors to produce sound. The user is responsible for selecting the correct printer model, reviewing the generated code and using it with the appropriate printer configuration.

Firmware, Bambu Studio and G-code behavior may change over time. Always verify correct operation after software or firmware updates.

Use of manually modified G-code, unsupported printers, or replacement of Machine G-code sections other than the dedicated sound block is entirely at the user's own risk.

---

## Author

**Ernesto Sorrentino**  
**DGVeLab**

Electronics • Firmware • Software • 3D Printing • Functional Engineering

---

## License

See the `LICENSE` file for details.
