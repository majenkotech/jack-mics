This is a modification of alsa_in to handle cleaner disconnecting of a USB device.

It also has a systemd configuration and wrapper script to automatically execute the
alsa_in replacement (alsa_mic) for a USB microphone that gets plugged in.

It is aimed at the SubZero microphones which are detected as /proc/asound/MICROPHONE
although other microphones can be used (you need to know the asound device name in that
case).
