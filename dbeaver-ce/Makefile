SHELL := /bin/bash

all: install clean

install:
	updpkgsums
	makepkg -si --noconfirm
	makepkg --printsrcinfo > .SRCINFO

clean:
	rm -rf src pkg
	rm -f *.pkg.tar
	rm -f *.tar.gz
