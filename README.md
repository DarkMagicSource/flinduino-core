# flinduino-core (mac-fix)

Downloadable core for the 'Flinders Flinduino' board in Arduino IDE

This is a personal fork to make the PIC32 toolchain work on modern macOS.
If you use Windows, Linux or macOS 10.14 or eariler, use the normal Flinduino version.

> **DISCLAIMER**: This software is provided "as is" with no ongoing support planned, updates will be made as they are needed for my own uses.

Tweaks to make this work on modern macOS are;
- Updating the PIC32 compiler to [this](https://github.com/CyberCastle/PIC32-MCU-Compiler/releases/tag/2.40-1) community compiled version for Intel x64 (Rosetta 2 automatically runs the binaries)
- Fix an out of bound error in `pic32/cores/pic32/cpp-startup.S`
- Remove unknown build flag `--save-gld` from `pic32/platform.txt`, `pic32/platformManual.txt` and `pic32/platformURL.txt`

## Instalation instructions

Instalation into the Arduino IDE is via the Boards Manager. Simply place this URL

https://raw.githubusercontent.com/DarkMagicSource/flinduino-core/master/package_flinduino_index.json

in the Preferences->Additional Boards Manager URLs: text field and then opening up the Boards Manager in the Tools->Board menu. 

> NOTE: you may need to force Arduino to redownload the package index, do this by running the command
`rm ~/Library/Arduino15/package_flinduino_index.json`

Tested on M1 with macOS 13.1 using Arduino IDE 1.8.19 and 2.0.3.
Extensive testing as not been conducted, only testing simple blink programs for now.



## Build Requirements

* [ANT](http://ant.apache.org/)

## Build Options

ant setup

ant github-release



