# Deepin Screenshot (Python)

Sometimes you just need to quickly grab part of screen, draw a bold red arrow with three question marks and paste it to chat. Deepin Screenshot is perfect tool for that case.

| Annotate | Selection |
| - | - |
| ![a](https://developer.run/pic/deepin-screenshot.png) | ![s](https://developer.run/pic/deepin-screenshot-selection.png) |

Fork of [snapshot tools](https://github.com/linuxdeepin-packages/deepin-scrot) for Linux Deepin, see [AUTHORS](./AUTHORS). Best Linux alternative for Lightshot with highlighting and annotating capabilities and multiple monitor support.



*Not to be confused with [Deepin Screenshot](https://www.deepin.org/en/original/deepin-screenshot/) which is rewrite of this tool using C++. I find Python version much more portable and open to modifications and improvements.*

[Original](https://github.com/linuxdeepin-packages/deepin-scrot) features:

* Simple and intuitive user interface like [Lightshot](https://app.prntscr.com/en/index.html)
* Fast, get screenshot in 2 button clicks
* Select window or any area
* Draw rectangle, ellipse, arrow, line or text onto the screen before taking the actual screenshot
* Save screenshot to file or clipboard
* Magnifier for precise pixel-perfect selection
* Show color under cursor
* Written in Python, easily portable between different Linux distros

[This fork](https://github.com/dmi3/deepin-screenshot) features:

* Fixed bug: screenshot included selection frame
* Fixed bug: empty (grey) magnifier
* Show color under cursor in HEX instead of RGB
* Middle click to copy color under cursor
* Button to open image in default viewer
* Support of multiple displays
* [Read more](https://developer.run/24)

Why this tool is better then [Shutter](http://shutter-project.org/):

* Shutter starts very slowly
* Shutter requires 5 unobvious actions to annotate image and copy it to clipboard `Edit Button→Draw...→Save→Edit Menu→Copy`
  - vs 2 clicks in Deepin Screenshot
* Shutter has no option to disable screenshot history
  - Creates clutter in filesystem
* Shutter has multiple windows
  - Creates clutter on desktop
* Shutter does not closes when screenshot is taken
  - Creates clutter in system tray

# Usage

* [Download](https://github.com/dmi3/deepin-screenshot/archive/master.zip) or clone this repository to any folder
* Ensure that you have Python and necessary dependencies installed `sudo apt-get install python-gtk2 python-xlib python-gi python-cairo`
* First generate mo files.
  Switch `deepin-screenshot` directory to execute updateTranslate.sh like below:
      ./updateTranslate.sh
* Quick start:
  Switch `src` directory to execute `deepin-screenshot` like below command:
      `cd ./src && ./deepin-screenshot`
* Assign a keyboard shortcut for `/path/to/deepin-screenshot/src/deepin-screenshot`   

