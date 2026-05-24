# Linux Loader is a program to play Sega Lindbergh games

## Linux Loader Loader Table of Contents

[TOC]

## Getting Started with Linux Loader

Sega Lindbergh ROMs typically come in the folder structure. The ROM is typically an executable ELF file contained within these ROM folders. For a full list of the executable ELF files, see the [Games List](#games-list) section.

Make sure to read Linux Loader's documentation for additional information on the emulator, [https://github.com/lindbergh-loader/lindbergh-loader/blob/master/docs/guide.md](https://github.com/lindbergh-loader/lindbergh-loader/blob/master/docs/guide.md).

### Games List

{{ read_csv('emulators/lindbergh-loader.csv') }}


### How to Install Linux Loader

Linux Loader is available both as an AppImage and a Flatpak on Linux. This page will cover how to utilize and install the AppImage. 

To download Linux Loader:

1. Open the Linux Loader GitHub releases page, [https://github.com/lindbergh-loader/linuxloader/releases](https://github.com/lindbergh-loader/linuxloader/releases) :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
2. Download the `linuxloader.AppImage` file
3. Move the downloaded AppImage to `$HOME/Applications`.
4. Right click the AppImage, {{ permissions }}
5. Double click the AppImage to run Linux Loader. 

### How to Play Games

1. Locate the associated ELF file for the game in the ROM folder. See the [Games List](#games-list) for a full list of the ELF file.
2. Right click the ELF file, click `Properties`, click `Permissions`, check `Execute`
    * This step is only required once per ROM.
3. Right click anywhere in the folder, click `Open Terminal Here`
4. Type the following command to launch the emulator:
    * `~/Applications/linuxloader.AppImage`
    * This will also automatically identify and launch the ELF file.

### How to Launch the Test Menu

In some cases, the test menu may be required to adjust settings for various purposes including disabling certain settings to allow some Sega Lindbergh games to run. This section will cover how to launch the test menu. 

1. Locate the associated ELF file for the game in the ROM folder. See the [Games List](#games-list) for a full list of the ELF file.
2. Right click anywhere in the folder, click `Open Terminal Here`
3. Type the following command to launch the emulator in test mode:
    * `~/Applications/linuxloader.AppImage -t`
4. When finished, exit out of the emulator. On the next launch, exclude `-t` to launch the ROM directly into the game.


## Linux Loader Tips and Tricks
