# Lindbergh Loader is a program to play Sega Lindbergh games. 

## Lindbergh Loader Table of Contents

[TOC]

## Getting Started with Lindbergh Loader

Sega Lindbergh ROMs typically come in the folder structure. The ROM is typically an executable ELF file contained within these ROM folders. For a full list of the executable ELF files, see the [Games List](#games-list) section.

Make sure to read Lindbergh Loader's documentation for additional information on the emulator, [https://github.com/lindbergh-loader/lindbergh-loader/blob/master/docs/guide.md](https://github.com/lindbergh-loader/lindbergh-loader/blob/master/docs/guide.md).

### Games List

{{ read_csv('emulators/lindbergh-loader.csv') }}


### How to Install Lindbergh Loader

1. Download the latest `lindbergh-loader.flatpak` to a folder of your choice.
2. Right click anywhere in the folder, click `Open Terminal Here`
3. Type the following command and press enter:
    * `flatpak install lindbergh-loader.flatpak -y`
    * The terminal will prompt for confirmation, type `y` and press enter.
5. When the installation is complete, type the following command to install the dependencies:
    * `flatpak install org.freedesktop.Platform.Compat.i386//24.08 org.freedesktop.Platform.GL32.default//24.08 -y`
6. Lindbergh Loader will now be installed. To run the emulator, type the following command:
    * `flatpak run com.github.lindberghloader`
    * To learn how to launch ROMs, see [How to Play Games](#how-to-play-games)


### How to Play Games

#### Permissions

By default the Lindbergh Loader Flatpak only has permissions to access ROMs in the `$HOME/Games` folder. In order to grant it access to additonal folders, you may use Flatseal. This section will cover how to do so.

1. In Desktop Mode, open Konsole.
2. Type the following command and press enter:
    * `flatpak install com.github.tchx84.Flatseal --user`
3. Once the installation is complete, open Flatseal.
4. Locate Lindbergh Loader on the left-hand side of the screen.
5. Scroll down to `Filesystem` on the right-hand side of the screen.
6. Under `Other Files`, type the path where your ROMs are located.
7. Once you have typed your path, Flatseal will auto-save, you may exit out and proceed to the next section to learn how to launch your ROMs. 

#### Games

1. Locate the associated ELF file for the game in the ROM folder. See the [Games List](#games-list) for a full list of the ELF file.
2. Right click the ELF file, click `Properties`, click `Permissions`, check `Execute`
    * This step is only required once per ROM.
2. Right click anywhere in the folder, click `Open Terminal Here`
3. Type the following command to launch the emulator:
    * `flatpak run com.github.lindberghloader`
    * This will also automatically identify and launch the ELF file.

### How to Launch the Test Menu

In some cases, the test menu may be required to adjust settings for various purposes including disabling certain settings to allow some Sega Lindbergh games to run. This section will cover how to launch the test menu. 

1. Locate the associated ELF file for the game in the ROM folder. See the [Games List](#games-list) for a full list of the ELF file.
2. Right click anywhere in the folder, click `Open Terminal Here`
3. Type the following command to launch the emulator in test mode:
    * `flatpak run com.github.lindberghloader -t`
4. When finished, exit out of the emulator. On the next launch, exclude `-t` to launch the ROM directly into the game.



## Tips and Tricks

### How to Launch Lindbergh Loader through ES-DE

ES-DE is a popular front-end for launching ROMs. This section will cover how to launch the Lindbergh Loader directly through ES-DE.

!!! danger "Load Times"

    Launching Lindbergh Loader through ES-DE may exponentially increase load times. This is the reason why there is no official support for Lindbergh Loader at this time.

1. In the `$HOME/ES-DE/custom_systems` folder, right click anywhere, click `Create New > Text File`, name it `es_find_rules.xml`
    * If you have already created a `es_find_rules.xml` file, skip to Step 3.
2. Right click the newly created `es_find_rules.xml` file, click `Open with Kate` or a text editor of your choice.
3. Paste the following text:

        <ruleList>
            <emulator name="LINDBERGH-LOADER">
                <!-- Sega Lindbergh emulator Lindbergh Loader -->
                <rule type="systempath">
                    <entry>com.github.lindberghloader</entry>
                </rule>
                <rule type="staticpath">
                    <entry>~/Applications/lindbergh</entry>
                    <entry>~/.local/share/applications/lindbergh</entry>
                    <entry>~/.local/bin/lindbergh</entry>
                    <entry>~/bin/lindbergh</entry>
                    <entry>/var/lib/flatpak/exports/bin/com.github.lindberghloader</entry>
                    <entry>~/.local/share/flatpak/exports/bin/com.github.lindberghloader</entry>
                </rule>
            </emulator>
        </ruleList>

4. Save the file and exit out.
5. In the `~/ES-DE/custom_systems` folder, right click anywhere, click `Create New > Text File`, name it `es_systems.xml`
    * If you have already created a `es_systems.xml` file, skip to Step 7.
6. Right click the newly created `es_systems.xml` file, click `Open with Kate` or a text editor of your choice.
7. Paste the following text:

        <systemList>
            <system>
                <name>lindbergh</name>
                <fullname>Sega Lindbergh</fullname>
                <path>%ROMPATH%/lindbergh</path>
                <extension>.elf .ELF .exe .EXE</extension>
                <command label="Lindbergh Loader (Standalone)">%STARTDIR%=%GAMEDIR% %EMULATOR_LINDBERGH-LOADER% %FILENAME%</command>
                <platform>lindbergh</platform>
                <theme>lindbergh</theme>
            </system>
        </systemList>

8. Save the file and exit out.
9. In the `ROMs` folder, create a `lindbergh` folder and place the Sega Lindbergh ROMs in this folder.
10. Sega Lindbergh ROMs can now be launched directly through ES-DE.
    * If the ROM you are trying to launch does not have a file extension or uses `.exe`, either add `.elf` to the file name or replace `.exe` with `.elf`. For example, with Afterburner, rename the `abc` file to `abc.elf`
    * For a full list of the ELF files, see [Games List](#games-list). Any file that does not explicitly write `.elf` needs `.elf` added to the file name in order for the ROM to be launched from ES-DE.