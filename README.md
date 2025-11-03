# The Unofficial RetroArch Better Defaults Project

This repository contains a collection of configuration files for RetroArch that aim to provide a better
out-of-the-box experience, such as:
* Settings for minimal input lag.
* A CRT shader enabled by default.
* Integer scaling when it's a close match for the display's resolution.
* Better button mappings for consoles with non-traditional controllers.
* Preconfigured core options to handle overscan.
* Overrides for game-specific enhancements.

## Installation
Copy the contents of the `config` folder into your RetroArch installation's
`config` folder. This will copy the emulator and game-specific settings.

The `better-defaults` folder contains the settings for RetroArch.
Copy its contents to the same location as `retroarch.cfg`:
  * On Windows, it's the RetroArch installation folder (`C:\RetroArch-Win64` by default.)
  * On Linux, it's `~/.config/retroarch`.
  * On MacOS, it's `~/Library/Application Support/RetroArch/config`.
  * On Android, it's `/storage/emulated/0/Android/data/com.retroarch/files`.

Open `better-defaults/main.cfg` in a text editor, read the comments (it won't take long!),
and make changes if necessary.

Finally, add this line to the **top** of `retroarch.cfg`:
```
#include "better-defaults/main.cfg"
```
