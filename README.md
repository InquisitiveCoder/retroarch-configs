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

Temporarily copy the contents of the `better-defaults` folder to the folder
that contains `retroarch.cfg`:
  * On Windows, it's the RetroArch installation folder (`C:\RetroArch-Win64` by default.)
  * On Linux, it's `~/.config/retroarch`.
  * On macOS, it's `~/Library/Application Support/RetroArch/config`.
  * On Android, it's `/storage/emulated/0/Android/data/com.retroarch/files`.

Then, open a terminal and run RetroArch using the `--apendconfig` option to
apply the relevant files:
```bash
retroarch --appendconfig="latency.cfg|ux.cfg|paths.cfg"
```
If you have an existing RetroArch installation with save files and save states,
you should remove `paths.cfg` from the list unless you intend to manually move
your saves and screenshots to the new paths.

Once RetroArch starts, you can delete `latency.cfg`, etc.
