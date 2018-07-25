SHELL := /bin/bash

all: install clean

install:
	updpkgsums
	makepkg -si
	makepkg --printsrcinfo > .SRCINFO

clean:
	rm -rf src pkg
	rm -f *.pkg.tar
