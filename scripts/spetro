#!/bin/bash
#
# generate spectrogram from input file
#
# example:
# sox glass.wav -n spectrogram -x 1024 -Y 1024 -o glass.png -h


if [ -z $1 ];then
	echo "Usage: $0 FILE.wav from audio/"
	exit 0
fi

FILE="$1"

sox ../audio/$FILE -n spectrogram -x 1024 -Y 1024 -h -o ../images/$FILE.$(date "+%F").png

echo "Done."
ls -lart ../images/$FILE.$(date "+%F").png
