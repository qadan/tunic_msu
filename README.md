# TUNIC MSU

MSU JSON for the TUNIC soundtrack.

## You will need:

* [msupcmplusplus](https://github.com/qwertymodo/msupcmplusplus/releases) - specifically, you need `msupcm.exe` from the latest release
* A copy of TUNIC. Any PC version should work; the macOS version will likely work too, but I couldn't tell you where the files are at
* A copy of the TUNIC soundtrack
* Yes, you will need _both the game and the soundtrack_
* [foobar2000](https://www.foobar2000.org/)
* The [foobar2000 component](https://vgmstream.org/downloads) for vgmstream must be installed in foobar2000

## Steps:

1. Extract both the `music_bank.bank` and `sfx_main.bank` files from TUNIC as .flac files. These files can be found wherever you installed TUNIC, under `Content\Secret Legend_Data\StreamingAssets`. To do this, open foobar2000, open each file, select all tracks with Ctrl-A, right click the selection, then pick "Convert", then "...". Under "Output format", use "FLAC", and "level 5". Under Destination, the File name pattern should be "%title%". Under "Processing", use "None". Click Convert
2. Place a copy of `tunic_msu.json`, and `msupcm.exe`, in the folder where the .flac files were extracted
3. Edit the .json to contain the full path to the song Early Birds .flac file in the soundtrack - or, alternatively, copy and paste Early Birds into the folder with the rest of the exported files. Either way, lines 396 and 400 need to be changed to point to the right location
4. Drag `tunic_msu.json` on top of `msupcm.exe` to run the conversion

Hey, now you have MSU files to attach to your ROM!

## Contact

Me if something is wrong. If you have song placement recommendations, they will be ignored. `fantallis#3161` on Discord.
