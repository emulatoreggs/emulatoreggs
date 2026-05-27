# umu launcher

This page will cover how to download and utilize umu launcher.

## umu launcher Tips and Tricks Table of Contents

[TOC]

***

## How To Install umu launcher
[Back to the Top](#umu-launcher-tips-and-tricks-table-of-contents)

1. Open the umu launcher GitHub repository, [https://github.com/Open-Wine-Components/umu-launcher/releases](https://github.com/Open-Wine-Components/umu-launcher/releases) :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
2. Download the latest `umu-launcher-#.#.#-zipapp.tar` file
    * The #.#.# refers to the version number, this may vary depending on when you are downloading umu launcher
3. Extract the `.tar` to a folder of your choice
4. Move the newly extracted `umu` folder to the `$HOME/.local/share` folder
5.  In the `$HOME` folder, right click the `.bashrc` file, click `Open with Kate` or a text editor of your choice
    * {{ hiddenfolders }}
6.  At the bottom of the `.bashrc` file, paste the following line:

      export UMU_HOME=$HOME/.local/share/umu
      export PATH=$UMU_HOME:$PATH

7.  Save and exit out of the `.bashrc` file
8. umu launcher will now be installed
    * If you had any terminals open previously, close these out and re-open them in order to use umu launcher through the command-line

## How to Utilize umu launcher with Applications

Make sure you have downloaded and installed umu launcher following the steps in the [How To Install umu launcher](#how-to-install-umu-launcher) section prior to reading this section.

1. Open Kate or a file editor of your choice
2. At the top of the file, write the following line:
    * `#!/bin/bash`
3. Press enter and use the following format:
    * `WINEPREFIX=~/PATH/TO/PFX GAMEID=0 PROTONPATH=GE-Proton umu-run /PATH/TO/APPLICATION.EXE`
4. Save the text file using the following format:
    * `APPLICATIONNAME.SH`
5. Right click the newly created text file, {{ permissions }}
6. To run the application, double click `APPLICATIONNAME.SH`