SHELL := /bin/bash

all: install clean

install:
	updpkgsums
	makepkg -si --noconfirm
	makepkg --printsrcinfo > .SRCINFO

clean:
	rm -rf src pkg
	rm -f *.pkg.tar
	rm -f blackfire-agent-*_x86_64
