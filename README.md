dmenu - dynamic menu
====================
dmenu is an efficient dynamic menu for X.


Requirements
------------
In order to build dmenu you need the Xlib header files.


Installation
------------
You must have `libxft-bgra` installed until the libxft upstream is fixed. (emoji support)

Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install

Running dmenu
-------------
See the man page for details.
Extra stuff added to vanilla dmenu:

- reads Xresources (ergo pywal compatible)
- alpha patch, which importantly allows this build to be embedded in transparent st
- can view color characters like emoji (libxft-bgra is required for this reason)
- `-P` for password mode: hide user imput
- `-r` to reject non-matching input
- dmenu options are mouse clickable


Fork from https://github.com/LukeSmithxyz/dmenu
