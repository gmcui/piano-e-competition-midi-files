# piano-e-competition-midi-files
All midi files in piano-e-competition

## Translated from original (Korean)

> All MIDI files were downloaded from [here](https://www.piano-e-competition.com/).
> 
> The web-crawling code is written in Kotlin and can be found in `src/main/kotlin/Main.kt`.
> 
> MIDI files downloaded directly from the web are located in the `download` directory.
> 
> The code to remove pedal data—while extending the duration of each note to account for the pedal—is written in Python and located at `python/MIDI_Pedal.py`.
> 
> The resulting files are stored in the `midi_without_pedal` directory.
> 
> ![image](https://user-images.githubusercontent.com/94269897/193013925-fcde1b39-aba5-4008-9085-a0813f072ca6.png)

## Reorganize and Rename

Since the original Piano-e-competition website is now offline, archived pages by Internet Archive Wayback Machine is used.  Here is the URL: https://web.archive.org/web/20190918170858/http://piano-e-competition.com/midi_2002.asp

Data for all performances are saved and edited to `csv/performances.csv`

MIDI files are renamed to include performer, composer, and title of the piece.  Detailed information of each piece is also saved to meta messages in the MIDI file.  New directories are created to save the MIDI files (symbolic links) in various organization schems, such as by year/round, or by composer/opus.

These files are stored in the `midi_with_title` directory.

### Notice

There may be mistakes in the processing of parsing the webarchive data. They will be corrected as they are found.
