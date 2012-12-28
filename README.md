SoundStreamer
=============

SoundStreamer is a Windows utility to capture default sound device output and pass it to external command. SoundStreamer launches the command specified in  'command.txt' file and writes PCM data to its stdin.

SoundStreamer was originally developed for streaming sound to Linux-based music server. In this case the external command should be like this:

    plink -pw password user@host play  -t raw  -c 2 -r 44100 -b 16 -e signed-integer --input-buffer 128 -

Place SoundStreamer.exe, plink.exe and command.txt in the same directory and launch SoundStreamer.exe.
