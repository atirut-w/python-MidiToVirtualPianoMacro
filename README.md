# Midi to Virtual Piano: Undawn Edition
This branch is specifically made for the game Undawn. Since it uses a different keymap, I decided to make a new branch for it. I may integrate this into the main branch later on, but that will have to wait until I clean it up a bit.

## Warning
This piano player portion of this program makes use of the python keyboard library which generates key presses programmatically. Antivirus software may (correctly) detect this as malicious activity! The executable were generated through a `pyinstaller --onefile`, which bundles a python program and its dependencies into a portable executable that requires no setup. Everyone is welcome to audit the source files and generate the executable for themselves. 

## Instructions
1. Go to the releases page and download the latest release for your operating system (Windows, Linux, etc.).
2. Extract `pyMIDI` and `playSong` and add some MIDI files to the same directory as the two programs.
3. Run `pyMIDI`. It will show you a list of songs from the directory it is in. Pick any song and it will generate a few files.
   1. `song.txt` is that `playSong` will read to play the song.
   2. `midiRecord.txt` is for debugging purposes. It shows that the converter did while converting the MIDI file.
   3. `SheetConversion.txt` is a human-readable version of `song.txt` that shows the notes in a more readable format.
4. Run `playSong`. It will wait for you to press the Delete key. Go to the program you want to play the song in and press the Delete key. The program will play the song for you.
