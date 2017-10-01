
alsa_mic:
	cc -o alsa_mic alsa_mic.c memops.c -I . -I /usr/include/jack -ljack -lm -lasound -lsamplerate

install:
	install -m 755 mic /usr/sbin
	install -m 755 alsa_mic /usr/bin
	install -m 644 microphone@.service /lib/systemd/system

clean:
	rm alsa_mic
