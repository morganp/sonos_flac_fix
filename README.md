
FlacConvert
===========

Given a top level music folder will search for and convert FLAC files that are above 48kHz and or above 16 bits. 

The fix version will use sox to convert them. This is **DESTRUCTIVE** it will replace the files **not** make copies.

**Status is still BETA**

The commands it runs on the music are:

    sox source_file -b 16 -r 48000 output_file


Requirements
--

Requires sox and the sox gem to be installed (using brew and ruby gems):

    brew install sox --with-lame --with-flac --with-libvorbis
    gem install soxi-wrapper


EXAMPLES
========

    report_sonos_flac_incompatible ~/Music

