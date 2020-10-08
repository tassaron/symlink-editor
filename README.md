# Symlink Editor

![Screenshot](/screenshot.png?raw=true)
![Screenshot](/screenshot2.png?raw=true)

A GUI Symlink Editor for Linux. Uses GTK+ 3 and Python 3+. Tested on Ubuntu 18.04 and 20.04.


# Installation:
1. If you're not on default Ubuntu (Gnome Desktop), then do `sudo apt install python3-gi`
2. Edit the .desktop file in this repo to have a valid filepath to the `symlink-editor` file.
3. After editing it, copy the .desktop file to `/usr/share/applications` and your desktop environment should detect it as an app.


# Features:
- Edit a symlink target or rename it
- Copy/duplicate symlinks
- Folder navigation (press icon in location bar to go up)
- Command-line options to integrate the program with another app


For example you can open an 'edit' dialog immediately for a file with: `symlink-editor /path/to/file`

Which could be used in a right-click context menu for example...
