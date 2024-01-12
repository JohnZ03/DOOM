http://sauparna.sdf.org/Doom/Compile_Doom

and open a blank window with the configuration Doom needs (note, the command name has an uppercase X)

Xephyr :2 -ac -screen 640x480x8
On my system I use display #:2 because a VNC server is attached to display #:1.

In another shell instance run Doom (where the binary has been built; linuxdoom-1.10/linux/), preceding the invocation to set the DISPLAY variable;

DISPLAY=:2
./linuxdoom