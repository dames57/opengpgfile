opengpgfile
===========

This is a small script to decrypt a file encrypted using GnuPG 
(GPG) into a somewhat secure temporary location and then open 
it for viewing using a sensible application. That is, a PDF 
file should open in a PDF viewer, an image in an image viewer, 
a word document in Libreoffice, etc etc..

Installation
------------

###Quick and dirty
Clone this repository and copy the script `bin/opengpgfile` to 
`/usr/bin` or `/usr/local/bin`.

###The better way
Get into the habbit of using [Stow](https://www.gnu.org/software/stow/) to manage the manually installed packages and scripts on you computer.

After you've installed stow, you could follow a process similar to this to get up and running with opengpgfile:

	mkdir /usr/local/stow
	cd /usr/local/stow
	git clone <this repository>
	stow opengpgfile

That's it. Stow will symlink 
`/usr/local/stow/opengpgfile/bin/opengpgfile` to 
`/usr/local/bin/opengpgfile`. This way, you can easily keep 
track of what you've manually installed on your system.

Requirements
------------

- gnupg
- mktemp
- xdg-open
- shred

