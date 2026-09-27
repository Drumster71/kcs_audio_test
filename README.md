# KCS Audio Test Files

## Overview

This repository contains KCS (Kansas City Standard) format test audio files generated for validating cassette encoding on vintage computers. The intention is for anyone with a suitable vintage computer, cassette drive, or drive emulator to load and test these files to verify the app beta can produce proper KCS encoded data which will run on an era correct 8-bit machine.

I have no authentic vintage computers on which to test these KCS audio files, and no experience with vintage code, so I'm hoping someone with a vintage machine can verify that these are indeed KCS compatible and that they can be read by their machine.

## Test Audio File

**File to test:** `kcs_test_300_baud.wav`

**Contains the following BASIC program:**

```basic
10 REM =================================
20 REM KCS TOOL COMPATIBILITY TEST
30 REM ANALOG SOFTWARE SOLUTIONS 2026
40 REM =================================
50 PRINT "KCS AUDIO LOAD SUCCESSFUL!"
60 PRINT "300 BAUD KANSAS CITY STANDARD"
70 FOR I = 1 TO 5
80 PRINT "TEST ROW "; I; " OK"
90 NEXT I
100 END
```

## Technical Specifications

### Character Encoding

- **Strict 7-bit Standard ASCII**: Uses only printable uppercase ASCII characters (0-9, A-Z, spaces, and basic punctuation)
- Vintage microcomputers (KIM-1, SYM-1, Ohio Scientific, SWTPC 6800, Processor Technology SOL-20, MSX, Acorn Atom, and CP/M systems) cannot parse modern UTF-8 or special characters
- **Universal BASIC Syntax**: Lines 10–100 use core Microsoft BASIC syntax supported across almost every 8-bit computer from 1976 through the 1980s
- **Dual-mode readable**: If loaded into a serial terminal program or TTY, it prints clean text. If loaded directly into a BASIC interpreter, it parses immediately as runnable code

### Audio Format

- **Encoding**: Kansas City Standard (CUTS / Byte Standard)
- **Baud Rate**: 300 Baud (1200 Hz Space / 2400 Hz Mark)
- **Channels**: Mono
- **Format**: PCM WAV

**Note:** Vintage 8-bit cassette hardware or ACIA/UART interfaces will fail to decode higher baud rates like 19,200 or 115,200.

## Testing Instructions

### Setup

- **Audio Volume**: Test play the audio back at 75%–80% volume (line level or via a cassette adapter) to prevent clipping or signal distortion in vintage tape input circuits
- **Download**: Download the `kcs_test_300_baud.wav` file from this repository
- **Connection**: Connect your PC audio output / headphone jack to your vintage computer's Cassette In or Tape Input port (or via a 3.5mm tape adapter inside a Datassette/Cassette recorder)

### Loading

- Set your vintage computer to load audio data (e.g., `LOAD`, `CLOAD`, or open your TTY / 300-baud terminal interface)
- Play the WAV file
- Upon completion, type `RUN` on your microcomputer to execute the loaded BASIC test program

## Context & Background

This tool was created to explore whether AI could help a musician write a simple program for converting standard text files onto cassettes. The goal is long-term archival storage—cassettes are essentially un-hackable and have excellent archival stability.

The conversion program (KCS Tool) has not yet been uploaded as it requires more thorough testing first.

I have included the source `.txt` file (`Vintage Test Payload Text - KCS Tool.txt`) for verification purposes.

**If you have a vintage computer and can test this file, your effort is greatly appreciated!**
