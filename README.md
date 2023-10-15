X11 RECORDING SCRIPTS
=====================

## Help

dia-h-xpdf

    Usage: dia-h-xpdf DIA-FILES...
    
    Convert DIA diagrams to pdf and display using xpdf(1).
    
    Dependencies: dia, xpdf

pulse-h

    Usage: pulse-h ...
    
    Helper script to select audio sinks and sources.
    
      -lI : List audio sources.  -tI : Test audio sources.
      -lO : List audio sinks.    -tO : Test audio sinks.
      
      -sI SRC : Set preferred pulse source.
      -cI     : Check the preferred pulse source is available.
      -gI     : Print preferred pulse source.
    
    Files: ~/.config/preferred_pulse_source
    Dependencies: mpv, ffmpeg, pulseaudio, normalize-audio

xrec-ffmpeg

    Usage: xrec-ffmpeg [-V][-s (stop)]
    
    Start/Stop recording, the recording sessions are saved in ~/REC
    with the start date. The PID is saved in ~/REC/pid.

xrec-menu

    Usage: xrec-menu [-l]
    
    Launch a small menu for accessing resources in a recording session.
    
      1. Script to read "SCRIPT.md"  (xfce4-terminal).
      2. Diagram files "*.dia"       (dia, xpdf).
      3. Slides "*.sent".            (sent)
      4. Autotypes "*.type".         (xdotool)
      5. URLs "*.url".               (google-chrome)
    
    Dependencies: 9menu

xrec-start

    Usage: xrec-start [-V]
    
    Start virtual desktop with the settings in "XREC", "../XRECP", "/etc/XREC".
    
      1. Create a directory in "/w".
      2. Copy files in STARTUPDIR to "/w".
      2. Launch a Xephyr session in ":1" with size SCREENSIZE.
      3. Launch "i3(1)" as the window manager in ":".
      4. If "WALLPAPER" set, will set it with "feh(1)".
      5. If "KEYBOARD" set, will set it with "setxkbmap".
    
    Dependencies: Xephyr, i3, feh, setxkbmap

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
