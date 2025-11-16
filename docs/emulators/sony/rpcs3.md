# RPCS3 is a Sony Playstation 3 Emulator.

## RPCS3 Table of Contents

[TOC]

## Getting Started with RPCS3

### How to Install RPCS3
[Back to the Top](#rpcs3-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

On Linux, the official packaging method for RPCS3 is an AppImage. 

To download RPCS3:

1. Open the RPCS3 website, [https://rpcs3.net/download](https://rpcs3.net/download) :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
2. Click the `Download` button in the `Linux` box.
3. Move the downloaded AppImage to `$HOME/Applications`.
4. Right click the AppImage, {{ permissions }}
5. Double click the AppImage to run RPCS3. 
6. (Optional) For easier maintenance, rename the AppImage to `rpcs3.AppImage`

## How to Configure RPCS3

### How to Configure Multiplayer
[Back to the Top](#rpcs3-table-of-contents)

??? info "Steam Input"
    {{ steaminput }} 

RPCS3 comes with a nifty auto-map feature that makes setting up multiplayer a breeze. To set up multiplayer, you simply need to enable the additional ports.

1. Open RPCS3
2. Open the `Pads` menu in the `Settings`
3. For each controller you are using for Player 2, 3, 4, etc, click the respective tab
    * You do not need to adjust any settings for Player 1
4. Under `Handlers`, select `SDL` for each player you are enabling
5. Under `Devices`
    * Player 2: `Steam Virtual Gamepad 2`      
    * Player 3: `Steam Virtual Gamepad 3`      
    * Player 4: `Steam Virtual Gamepad 4`
    * Player 5: `Steam Virtual Gamepad 5`
    * Player 6: `Steam Virtual Gamepad 6`
    * Player 7: `Steam Virtual Gamepad 7`
6. Using `Player 2` as an example:
    * On the `Player 2` configuration screen, after you have selected the appropriate `Device` and `Handler`, click `Refresh` to the right of `Handler`
7. After you are finished enabling any additional players, click `Save` and you may open your game either directly as a shortcut in Steam or through ES-DE and Pegasus
8. (Optional) You may need to re-arrange the controller order in Game Mode for your controllers to function as expected. See [How to Re-Arrange the Controller Order](../../controls-and-hotkeys/steamos/external-controllers.md#how-to-re-arrange-the-controller-order) to learn how

***

### How to Set up the Motion Sensor with External Controllers
[Back to the Top](#rpcs3-table-of-contents)

The PlayStation 3 controller, or the DualShock 3 notably had "Sixaxis". Sixaxis refers to the motion sensor used in a handful of games. One of the more popular games that utilized Sixaxis was Folklore. For a full list of games, see [https://www.giantbomb.com/sixaxis-support/3015-5310/games/](https://www.giantbomb.com/sixaxis-support/3015-5310/games/).

RPCS3 has implemented support to allow emulating the Sixaxis through evdev, which exposes the gyro in a large variety of modern controllers (including the Nintendo Switch Pro Controller, 8BitDo Ultimate Controller, and the DualSense). 

At this time, the Steam Deck gyro **cannot** be used. But if you own one of these controllers, you may emulate the Sixaxis through RPCS3.

??? info "Steam Input"
    {{ steaminput }} 

1. If Steam is open, exit out of Steam :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
    * You may exit out of Steam a couple of different ways:
        * Right click the `Steam` icon in your taskbar and click `Exit Steam`
        * Open Steam, click the `Steam` button in the top left, click `Exit`
        * Open a terminal (Konsole) and enter `killall -9 steam`
        * Do note that clicking the the `X` button in the top right of the Steam window **will not** exit out of Steam
    * If using a Steam Deck, your controls will switch to `Lizard Mode`. Use `L2` to right click, `R2` to left click, and the `Right Trackpad` to move the mouse
        * You may also connect an external keyboard and mouse
2. Connect your controller using bluetooth
3. Open `RPCS3` 
4. Click `Pads` at the top
5. Under the `Player 1` tab, click the Dropdown box below `Devices` and select your controller
    * To switch back to the default controller layout, make sure `Steam` is open and select `Steam Virtual Gamepad 1`
6. Click `Save`, and exit out of RPCS3

#### Game Mode

1. In Game Mode, connect your controller
2. Select your PlayStation 3 game 
3. On the `Play` screen, select the `Controller` icon to the right of the screen 
4. Select your controller tab at the top
5. Click `Reorder Controllers` and move your external controller to the top
6. Click the `Gear` icon to the right, and click `Disable Steam Input`
    * You may need to restart first for this setting to properly apply
7. Your controller's gyro will now work for this selected game, repeat as needed for your other games

#### Post-Configuration

To restore the default controls:

1. Open RPCS3
2. Click `Pads` at the top
3. Under the `Player 1` tab, click the Dropdown box below `Devices` and select `Steam Virtual Gamepad 1`
4. Select `SDL` under `Handlers`
5. Click `Save`, and exit out of RPCS3

(Optional) To restore Steam Input:

1. Select your PlayStation 3 game 
2. On the `Play` screen, select the `Controller` icon to the right of the screen 
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/468d63e3-534c-4270-ac61-06e167d6df48" height="300">
3. Select your controller tab at the top
    * <img src="https://github.com/dragoonDorise/EmuDeck/assets/108900299/b51a1405-9cdf-4ba3-bebf-db817f057f63" height="300">
4. Click the `Gear` icon to the right, and click `Enable Steam Input`
    * You may need to restart first for this setting to properly apply
5. The controls will be reverted to Steam Input and the Steam Deck controls will be restored

***

### How to Roll Back RPCS3 to an Older Version
[Back to the Top](#rpcs3-table-of-contents)

1. Download the version of the emulator you would like to use from RPCS3's Builds page: [https://rpcs3.net/compatibility?b](https://rpcs3.net/compatibility?b)
2. Move the downloaded emulator from Step 1 to `/home/deck/Applications`
3. **(Optional)** Rename or delete the original emulator file
4. Right click the newly downloaded emulator, click `Properties`, click `Permissions`, check `Is executable`
5. Your games will now launch using the version of the emulator you downloaded

***

### How to Configure Language Settings
[Back to the Top](#rpcs3-table-of-contents)

#### In-Game

1. In Desktop Mode, open RPCS3
2. At the top, click `Configuration`, click `System`
3. Below `Console Language`, select your preferred language in the drop-down menu


***
