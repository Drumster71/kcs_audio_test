I have used a range of AI models to create a simple tool to convert standard .txt and .docx text files into KCS (Kansas City Standard) format .wav files, which can be stored on magnetic tape or other physical audio media.
I have no authentic vintage computers on which to test these KCS audio files, and no experience with vintage code, so I'm hoping someone with a vintage machine can verify that these are indeed KCS compatible files,
and that they can be read by their machine. 
I have included the source .txt file; 'Vintage Test Payload Text - KCS Tool' for verification purposes.

File to test: kcs_test_300_baud.wav

Contains the following code:
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

Instructions (from Google Gemini) :
Strict 7-bit Standard ASCII: Uses only printable uppercase ASCII characters (0-9, A-Z, spaces, and basic punctuation).
Vintage microcomputers (KIM-1, SYM-1, Ohio Scientific, SWTPC 6800, Processor Technology SOL-20, MSX, Acorn Atom, and CP/M systems) cannot parse modern UTF-8 or special characters.
Universal BASIC Syntax: Lines 10–100 use core Microsoft BASIC syntax supported across almost every 8-bit computer from 1976 through the 1980s.
Readable as Code or Raw Terminal Text: If loaded into a serial terminal program or TTY, it prints clean text. If loaded directly into a BASIC interpreter, it parses immediately as runnable code.

Recommended Encoding Settings for Vintage Testing:
Baud Rate: Set the tool selector to 300 Baud. Standard Kansas City Standard (CUTS / Byte Standard) specifies 300 Baud (1200 Hz Space / 2400 Hz Mark). 
Vintage 8-bit cassette hardware or ACIA/UART interfaces will fail to decode higher baud rates like 19,200 or 115,200.
⦁	Audio Volume: Test play the audio back at 75%–80% volume (line level or via a cassette adapter) to prevent clipping or signal distortion in vintage tape input circuits.
⦁	Download the generated kcs_test_300_baud.wav file.
⦁	Connect your PC audio output / headphone jack to your vintage computer’s Cassette In or Tape Input port (or via a 3.5mm tape adapter inside a Datassette/Cassette recorder).
⦁	Set your vintage computer to load audio data (e.g., LOAD, CLOAD, or open your TTY / 300-baud terminal interface).
⦁	Play the WAV file.
⦁	Upon completion, type RUN on your microcomputer to execute the loaded BASIC test program.

Your effort is greatly appreciated, I am not a coder, this is simply a fun little idea I had several years ago, and was curious to see if AI was able to help a musician to write a simple program that could backup
text files onto cassettes. I have hundred of cassettes, I like the way they're essentially un-hackable, and have excellent archival stability.
I'm not confident enough to upload the program (KCS Tool) just yet, I would like to test it thoroughly first. 
