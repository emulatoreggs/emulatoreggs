# Dolphin is a Nintendo GameCube and Wii Emulator.

## Dolphin Table of Contents

[TOC]

## Getting Started with Dolphin

### How to Install Dolphin
[Back to the Top](#dolphin-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

Dolphin is available as an **unofficial** Flatpak on Linux. This page will cover how to utilize and install the Flatpak. 

To download Dolphin:

1. In Desktop Mode, open Konsole or a terminal of your choice
2. If you have not already added the Flathub user repo, type the following and press enter:
    * `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo --user`
3. Type the following and press enter:
    * `flatpak install org.DolphinEmu.dolphin-emu --user -y`
4. Type the following two lines, one at a time, and press enter after each line:
    * `flatpak override org.DolphinEmu.dolphin-emu --filesystem=host --user`
    * `flatpak override org.DolphinEmu.dolphin-emu --share=network --user`

If you have Discover installed, you may also use Discover to install Dolphin. Make sure you have the Flathub repo added (Step 2 in the section above). 

## Dolphin Tips and Tricks

### How to Enable HDR
[Back to the Top](#dolphin-table-of-contents)

With the latest Dolphin update, HDR can now be used on Steam Deck OLEDs. Here's how to enable it.

1. Switch to Desktop Mode.
2. Open Konsole.
3. The following command will set a sudo password. If this is your first time setting a sudo password, make sure it is secure and that you **do not** forget it. if you have already set a sudo password, skip to Step 4.
    * `passwd`
    * Konsole will prompt you to create a password, any characters typed here will not display in the terminal. Once you have typed a password, press enter and Konsole will ask you to type it again to confirm. 
    * If the commands after this step request a sudo password, type the password you created here for the respective step. 
4. Type the following command and press enter: 
    * `flatpak install org.freedesktop.Platform.VulkanLayer.gamescope -y`
5. The Flatpak Gamescope will now be installed.
6. In Desktop Mode, open the Dolphin emulator.
7. Click the `Graphics` button
8. Click the `Enhancements` tab
9. Check `HDR Post-Processing`
10. Click the `Post-Processing Effect` drop-down menu and select `PerceptualHDR` or `AutoHDR` depending on your preference.
    * See the [latest Dolphin blog](https://dolphin-emu.org/blog/2024/04/30/dolphin-progress-report-february-march-and-april-2024/#hdr-enhancements-50-19931-add-autohdr-post-process-shader-by-filoppi-and-50-21232-add-hdr-to-metal-perceptual-hdr-by-samb) for more info on the difference between the two
12. HDR will now be enabled in **Game Mode**.


***

### How to Switch Dolphin to the Development Branch
[Back to the Top](#dolphin-table-of-contents)

RetroAchievements was recently added to Dolphin but can only be used in the development branch until it has been tested thoroughly for public release. 

If you are interested in using the development branch to test RetroAchievements or any other Dolphin feature before it is officially released, you may do so by following the steps in this section. 

??? warning 

    Do keep in mind these builds are experimental and may have bugs. If you are using the development build and request support, make sure to include that you are using the development build. If you are using the development build and would like to use netplay, the other individual must be on the identical development build version. It is highly recommended you use the stable builds instead if you would like to use netplay. 

#### How to Switch Dolphin to the Development Branch

1. In Desktop Mode, open Konsole or a terminal of your choice
2. Type the following and press enter:
     * `flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo --user`
3. Type the following and press enter:
    * `flatpak install flathub-beta org.DolphinEmu.dolphin-emu --user -y`
4. The development version of Dolphin has now been installed. To switch to the development branch as the primary version of Dolphin, type the following and press enter:
    * `flatpak make-current org.DolphinEmu.dolphin-emu beta --user`
  
To switch back to the "Stable" build ("Releases" on the Dolphin website), type the following and press enter:

`flatpak make-current org.DolphinEmu.dolphin-emu stable --user`

If you had Dolphin installed at the system level, you will need to type the following instead:

`sudo flatpak make-current org.DolphinEmu.dolphin-emu stable`

***
