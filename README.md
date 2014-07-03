README - whistle

Prerequisites:
--------------

Perl Modules:
    
        - MP3::Info           (archlinux-package: perl-mp3-info)
        - Curses::UI          (archlinux-package: perl-curses-ui)
        - File::MimeInfo      (archlinux-package: perl-file-mimeinfo)
        - Ogg::Vorbis::Header (aur-package: perl-ogg-vorbis-header)

Programs:

        - mplayer (mpg123 earlier)


What works? a.k.a. Features:
----------------------------

        - full MP3/OGG play/stop/next/prev/seek/shuffle support
        - progressbar
        - playlists
        - multi-select for playlist-editing
        - better and finer granulated equalizer (10 band)


What's to come?
---------------

        - a lot of bugfixes for sure
        - color support
        - tab completition
        - mp3 tag write support
        - burn playlist 2 iso or cd
        - ...
        - your feature request?


Usage:
------

whistle must be started within a fully functional terminal.

The first step is to add a music directory with 'A'. The standard
usage scenario then is to select what you want to play and press 'P'.



About:
------

whistle aims to be a very minimalistic and basic audio player.
Currently it can play mp3- and ogg-vorbis-files.

Basically, whistle is a nifty front-end to mplayer, which it's
based on. Without mplayer, there would be no whistle. The earlier
mpg123 back-end is now completely done by mplayer.


Thanks:
-------
 - all the people testing and helping me to improve whistle :)
   (kmandla, matthew cox, smiszym, ...)
 - all developers behind mpg123, mplayer and mpv
 - all developers from Curses and Curses::UI
 - all developers from MP3::Info
 


If you really like this tool, feel free to tip me via [Gittip][tip].

[![Gittip](http://img.shields.io/gittip/ap0calypse.svg)](https://www.gittip.com/ap0calypse/)

[tip]:https://www.gittip.com/ap0calypse/
