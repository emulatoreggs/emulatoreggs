# melonDS is a Nintendo DS emulator.

Website: [https://melonds.kuribo64.net/](https://melonds.kuribo64.net/)

melonDS' FAQ: [https://melonds.kuribo64.net/faq.php](https://melonds.kuribo64.net/faq.php)

GitHub: [https://github.com/melonDS-emu/melonDS](https://github.com/melonDS-emu/melonDS)

Compatibility List: [https://melonds.kuribo64.net/board/forum.php?id=3](https://melonds.kuribo64.net/board/forum.php?id=3)

## melonDS Table of Contents

[TOC]

## Getting Started with melonDS

### How to Install melonDS
[Back to the Top](#melonds-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

melonDS is available both as an AppImage and a Flatpak on Linux. This page will cover how to utilize and install the Flatpak. 

To download melonDS:

1. Open your distro's software manager.
    * {{ discover }}
2. Search for "melonDS" and click "Install" on the top right of the software page For melonDS
3. Open Konsole or a terminal of your choice
4. Type the following command and press enter after typing the command:
    * `flatpak override net.kuribo64.melonDS --filesystem=host --user`
    * {{ flatseal }}
5. melonDS will now be installed and properly configured


## melonDS Tips and Tricks
[Back to the Top](#melonds-table-of-contents)

***


### Open Source BIOS
[Back to the Top](#melonds-table-of-contents)

The open source BIOS is **enabled by default** for melonDS. This means that BIOS for Nintendo DS games is **optional**. However, some games may not perform as expected with the open source BIOS or you may need additional features provided by console dumped BIOS. You may also prefer to use DSI BIOS which allow you to play DSIWare games. 

In order to use console dumped BIOS, you may place the files required into the `Emulation/bios` folder. You will also need to enable `Use external BIOS/firmware files` in the melonDS GUI. 

![melonDS Open Source BIOS](../../assets/melonds-open-source-bios.png)

***

### How to Configure Multiplayer
[Back to the Top](#melonds-table-of-contents)

This section is strictly referring to local multiplayer. melonDS multiplayer on the Steam Deck can only be done in Desktop Mode.

1. In Desktop Mode, open melonDS
2. Click `System`, click `Multiplayer`, `Launch new instance`
3. On each window of melonDS, click `Config`, `Input and hotkeys`
4. In the drop-down menu to the right of `Joystick`, select your controller
    * Steam Deck/Player 1: `Microsoft X-Box 360 pad 0`
    * Player 2: `Microsoft X-Box 360 pad 1`
    * Player 3: `Microsoft X-Box 360 pad 2`
    * Player 4: `Microsoft X-Box 360 pad 3`
5. Open the game in each melonDS window and you will be able to play multiplayer

You can determine which melonDS window corresponds to what player by looking at the menu bar at the top. Each new melonDS window will have a corresponding `(#)`.

***


### How to Use Cheats
[Back to the Top](#melonds-table-of-contents)

**Note:** melonDS does not currently support importing cheats from a database file.

#### How to Enable Cheats in melonDS

1. Open melonDS
2. Click `System` at the top
3. Check `Enable cheats`
    * <img src="https://user-images.githubusercontent.com/108900299/220514789-7511568d-4806-4528-8521-ea1d6e35b989.png" height="300">

#### How to Download the Cheats Database

1. Open [https://db.universal-team.net/ds/ndsi-cheat-databases](https://db.universal-team.net/ds/ndsi-cheat-databases), right click `cheats.xml`, and click `Save As`
2. Place it in `Emulation/storage/melonds/cheats`
    * This folder placement is optional, you may place it wherever you want
3. To view, right click `cheats.xml`, open with a text editor of your choice

#### How to Use the Cheats Database

**Note:** It's recommended you do this in Desktop mode so you can easily copy from the cheats database into MelonDS. After adding cheats, you can use MelonDS in Game Mode. 

1. Open the `cheats.xml` you downloaded from the `How to Download the Cheats Database` section
2. `CTRL` + `F` the game you are adding cheats to
3. Copy the blocks of alphanumerical strings between the two `<codes> <codes>` for your respective cheat
    * Example: <img src="https://user-images.githubusercontent.com/108900299/220517493-9305654f-660e-4845-8210-ea1da61ce2b2.png" height="300">
4. Open MelonDS
5. Open a ROM
6. Click `System` at the top
7. Click `Setup cheat codes`
8. Create a `New Category`, you may name it whatever you would like
9. Click `New AR Code`
10. Match the name of the AR Code to the cheat you located in Step 3
   * The name is flexible, you may name it whatever you would like
11. Paste the code you copied from Step 3, it will appear as red text
13. Format the cheat so there are two blocks of code per line
    * Original: <img src="https://user-images.githubusercontent.com/108900299/220517044-dc4c547b-7a13-4a42-aa34-c3f36786c320.png" height ="300">
    * Corrected: <img src="https://user-images.githubusercontent.com/108900299/220516960-47147c37-d914-4ced-9893-f5b9c9e47781.png" height="300">
14. Some cheats are automatically activated, others will require a button combo. Look at the `cheats.xml` file to see if a button combo is required to activate your cheat

***

### How to Set Up DSIWare
[Back to the Top](#melonds-table-of-contents)

The Nintendo DSI requires DSI specific BIOS. Place **all** of the files from the list below **directly** in `Emulation/bios`.

* `dsi_bios9.bin`
* `dsi_bios7.bin`
* `dsi_firmware.bin`
* `dsi_nand.bin`

**Note:** 

* The BIOS must be named exactly as above. BIOS with any deviations from the above **will not** work. Make sure you have the proper casing, characters, and spelling. 
* BIOS must be placed in `Emulation/bios`. If you create a sub-folder, the BIOS will not be picked up and Nintendo DSI games **will not** work. 

***

**Preface:** Generally, DSIWare games are named `00000000` with no file extension. This section assumes you have these types of DSIWare ROMs. 

1. Place your DSI BIOS in `Emulation/bios`
2. Place your DSIWare ROMs in `Emulation/roms/nds`
3. Right click the DSIWare ROM in `Emulation/roms/nds`, click `Rename`, rename it from `00000000` to `GAMENAME.app`
    * Replace `GAMENAME` with the name of the DSIWare game
    * For example:
        * Original file name: `00000000`
        * Updated file name: `X-Scape.app`
4. In Desktop Mode, open melonDS
5. At the top, select `Config`, `Emu Settings`
6. On the `General` tab, change the `Console type` to `DSi (experimental)`
    * ![How to Set Up DSIWare 1](../../assets/how-to-set-up-dsiware-1.png)
7. On the `DS-mode` tab, check `Use external BIOS/firmware files`, close out of this menu
    * ![How to Set Up DSIWare 2](../../assets/how-to-set-up-dsiware-2.png)
8. At the top, select `System`, `Manage DSi titles`
9. On the `DSi Title Manager` screen, select `Import title`
10. Select your `GAMENAME.app` as the `Executable`
11. Under `Metadata`, select `Download from NUS`, close out of this menu
12. Select `File`, `Boot Firmware`
13. Select your newly-installed DSiWare game and start playing

***

## Steam Deck

### How to Configure Settings
[Back to the Top](#melonds-table-of-contents)

#### Game Mode

If you are playing in Game Mode, make sure you have the correct "Steam Input" profile applied.

While in game, press `Select` + `R3` to exit full screen. While melonDS is windowed, you will have access to the settings at the top of the screen. Adjust these options to your liking. After you have made your changes, press `Select` + `R3` again to switch melonDS back to full screen. 

After you have made your changes and you are ready to exit your game, **do not** use the `STEAM` butto to exit out of the game. If you use the `STEAM` button, any changes you have made will be reverted. 

Press `Select` + `R3` again to exit full screen. In the top right, click `File`, click `Quit`. You will only need to do this when you are changing settings. Otherwise, you may simply use the `STEAM` button as usual. 

#### Desktop Mode

In Desktop Mode, open melonDS. Adjust any options to your liking. In the top right, click `File`, click `Quit`.

**Do not** click the `X` button in the top right to exit out of melonDS. If you use the `X` button, any changes will be reverted.

***

### How to Configure Language Settings
[Back to the Top](#melonds-table-of-contents)

#### In-Game

Some games may not have language options. For a full list of which games have language options, download the DS Database from GamesTDB, [https://www.gametdb.com/DS/Downloads](https://www.gametdb.com/DS/Downloads) and open it in a text editor of your choice. 

Before proceeding with the below section, you will need to place Nintendo DS BIOS in the `Emulation/bios` folder.

1. In Desktop Mode, open melonDS
2. At the top, click `Config`
3. Click `Emu settings`
4. Click `DS-Mode`, check `Use external BIOS/firmware files`
5. Close out of the `Emu settings` window
6. Click `File`, click `Boot firmware`
7. Click the DS icon at the bottom of the screen
8. Click the gear icon
9. Click the globe icon
10. Select your preferred language


***