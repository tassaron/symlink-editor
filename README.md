# Symlink Editor

A graphical Symlink Editor for Linux. Uses GTK 3 and Python 3. Tested on Ubuntu 18.04, 20.04, and 22.04, but it should work anywhere you can install GTK bindings for Python.


![Screenshot](/screenshot.png?raw=true)

```
usage: symlink-editor [-h] [-new] [-dir DIR] [-leaveopen] [path-to-edit]

graphically manage symbolic links

positional arguments:
  path-to-edit  open an edit dialog for this path

options:
  -h, --help    show this help message and exit
  -new          open a dialog to create a new link
  -dir DIR      start in this path instead of the default
  -leaveopen    leave main window open after editing
```


## Features:

- Notice broken symlinks easily (red highlighting)
- Edit a symlink target or rename it
- Copy/duplicate/move symlinks
- Folder navigation (press icon in location bar to go up)
- Use with "Open with..." in a file manager
- Runnable as root with `sudo` (please be careful!)


## Installation:
1. If you're not on default Ubuntu (Gnome Desktop), then run `sudo apt install python3-gi` to install Python support for GTK
1. *Recommended on Ubuntu:* Create a folder called "bin" in your home folder and extract this code in that folder. This is a standard location for weird user-installed apps such as this.
1. Edit the symlink-editor.desktop file to have a valid filepath to the `symlink-editor` file (and the icon you want)
1. Copy/move the symlink-editor.desktop file to `/usr/share/applications` and your desktop environment's app launcher should detect it
1. If you can't run the file, try marking it as executable (using properties window or `chmod +x` from terminal)


## Development
* Because the GTK widgets are defined in Python code in one giant file, the code is not readable by mortal eyes. But it *is* technically being maintained as of 2022. Pull requests are welcome, but beware :)
