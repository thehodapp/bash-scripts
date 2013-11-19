bash-scripts
============

A few useful random bash scripts I've written.

### chkcd

Outputs the MD5 sum of a CD in regards to an ISO filesize (assumed to have been burned to the CD).  
This is used to check the integrity of the data burned to a CD.

Usage: chkcd [-d DEVICE] FILENAME

### cplay

Requires: **cmus**  
Tests if cmus is running and starts it if it isn't.  
Else it toggles play/pause. This command will break if you rename it to
something containing "cmus".

Note: I use this with a shortcut key to start and play cmus in a terminal

### flac2mp3

Source: **Arch wiki**  
Converts FLAC files to mp3

### irc-start

Requires: **irssi**  
Starts irssi

**Note:** I use this with a shortcut key to start irssi in a terminal

### mkalias

Usage: mkalias ALIAS=EXPRESSION  
Makes alias permanent by writing to .bash_aliases contained in home directory.

### ripcd

Requires: cd-paranoia, picard  
Rips a cd and, converts to wave, and then encodes in:  
-f flac at level 8  
-o 320kb/s ogg (level 9)  
-m VBR mp3 at highest quality (level 0)  
Finally, opens picard program so that you can add artist, title, etc. tags

Usage: ripcd [-f|-o|-m]

### update-chromium-pdf

Normally, Chromium cannot open PDF files in the browser because only Chrome
provides the proprietary plugin to open them. This script will download the
PDF library and add it to Chromium. You will need to provide your password to
install the library in the correct directory.

