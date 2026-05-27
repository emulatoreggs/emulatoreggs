# Waydroid is a container application to run Android on Linux

!!! danger "Advanced Configurations"

    Waydroid at this present time involves using a script which requires some level of comfort in the terminal. If using SteamOS, Waydroid installations are wiped on major system updates. When updates occur, the script will first need to be updated by the maintainer before it can be re-installed by the user. Over time, with kernel and system updates, Waydroid should become easier to install. 

## Waydroid Table of Contents

[TOC]

## Getting Started with Waydroid

### How to Install Waydroid
[Back to the Top](#waydroid-table-of-contents)

The following steps use the `SteamOS Android Waydroid Installer`. For the GitHub repository, see [https://github.com/ryanrudolfoba/steamos-waydroid-installer](https://github.com/ryanrudolfoba/steamos-waydroid-installer)

1. Open Konsole or a terminal of your choice :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
2. Type the following commands one at a time to clone the repository:
    * `mkdir -p $HOME/Applications/GitHub && cd $HOME/Applications/GitHub`
    * `git clone --depth=1 https://github.com/ryanrudolfoba/steamos-waydroid-installer`
3. To run the script, type the following commands one at a time:
    * `cd $HOME/Applications/GitHub/steamos-waydroid-installer`
    * `chmod +x steamos-waydroid-installer.sh`
    * `./steamos-waydroid-installer.sh`
    * The script will automatically install Waydroid, installation may take a few minutes.
4. If on SteamOS, a Waydroid launcher will be automatically added to your non-Steam games library in Steam. You may return to Game Mode to launch Waydroid

## Waydroid Tips and Tricks

