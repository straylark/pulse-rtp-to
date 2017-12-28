play audio from one machine to another over RTP with pulseaudio

## how to use it

(on audio-playing machine)

    $ git clone https://github.com/straylark/pulse-rtp-to
    $ ./pulse-rtp-to/pulse-rtp-to target-host

(on target-host)

    $ vlc rtp://@:47777

(back on audio-playing machine)

    $ PULSE_SERVER=/run/user/$UID/pulse/native mpv song.mp3
