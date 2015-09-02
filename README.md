About:
------

whistle aims to be a very minimalistic and basic audio player.
Currently it can play mp3, flac and ogg files.

Basically, whistle is a nifty front-end to mplayer, which it's
based on. Without mplayer, there would be no whistle. The earlier
mpg123 back-end work is now completely done by mplayer.


Latest screenshot:
------------------

![screenshot whistle](screenshot.png "Screenshot")


Prerequisites:
--------------

Perl Modules:
    
        - MP3::Info           (archlinux-package: perl-mp3-info)
        - Curses::UI          (archlinux-package: perl-curses-ui)
        - File::MimeInfo      (archlinux-package: perl-file-mimeinfo)
        - Ogg::Vorbis::Header (aur-package: perl-ogg-vorbis-header)
        - Audio::FLAC::Header (aur-package: perl-audio-flac-header)

Programs:

        - mplayer (mpg123 earlier)


Installation:
-------------

ArchLinux:
    packer -S mplayer perl-ogg-vorbis-header perl-audio-flac-header perl-mp3-info perl-curses-ui perl-file-mimeinfo whistle-git
    
(you maybe need to replace 'packer' with your custom AUR-helper (yaourt, clyde, ...)

Slackware:

Unfortunately, there is no prepackaged version of whistle for Slackware, but it can be installed following these steps (all listed packages are either needed by whistle or are dependencies of each other) :

    1. install sbopkg (http://www.sbopkg.org/downloads.php,-> installpkg sbopkg-version-noarch-1_cng.tgz) to install custom libs and programs
    2. run sbopkg and sync with slackbuilds.org (Sync with remote repository)
    3. install the following perl-packages:
        - perl-Audio-FLAC-Header
        - perl-Curses
        - perl-Curses-UI
        - perl-File-Which
        - perl-IPC-Run3
        - perl-IPC-System-Simple
        - perl-MP3-Info
        - perl-Module-Build
        - perl-Ogg-Vorbis-Header-PurePerl
        - perl-Probe-Perl
        - perl-TermReadKey
        - perl-Test-Script
        - perl-ExtUtils-depends
        - perl-ExtUtils-makemaker
        - perl-ExtUtils-pkgconfig
        - perl-file-basedir
        - perl-file-desktopentry
        - perl-file-mimeinfo
    4. clone the git repository: (git clone https://github.com/ap0calypse/whistle.git)
    5. From here on, you have 2 options:
        a. you either install the Perl-module for Ogg-Vorbis-Header via CPAN
        b. you run the following command in the cloned repository to make whistle use the Ogg-Vorbis-Header-PurePerl module 
        -> sed -i 's/Ogg::Vorbis::Header/Ogg::Vorbis::Header::PurePerl/g' whistle
    6. run whistle and enjoy :)


What works? a.k.a. Features:
----------------------------

        - full MP3/OGG/FLAC play/stop/next/prev/seek/shuffle support
        - progressbar
        - playlists
        - multi-select for playlist-editing
        - better and finer granulated equalizer (10 band)
        - per-song/album-equalizer (meaning: individual equalizer settings 
          for each title/album/artist)


What's to come?
---------------

        - a lot of bugfixes for sure
        - shuffle by artist/album
        - equalizer presets
        - color support
        - mp3 tag write support
        - burn playlist 2 iso or cd
        - ...
        - your feature request?


Usage:
------

whistle must be started within a fully functional terminal.

The first step is to add a music directory with 'A'. The standard
usage scenario then is to select what you want to play and press 'P'.


Thanks:
-------
 - all the people testing and helping me to improve whistle :)
   (kmandla, matthew cox, smiszym, ...)
 - all the supportive people of the arch-community :)
 - all developers behind mpg123, mplayer and mpv
 - all developers from Curses and Curses::UI
 - all developers from MP3::Info
 - all developers from Ogg::Vorbis::Header
 - all developers from Audio::FLAC::Header
 


If you want to give me some crypto-credit, please use this adress:

  - DogeCoin:   DGA1bAaftiYCT1ndTLzHMmyty9rs8bPmFR
