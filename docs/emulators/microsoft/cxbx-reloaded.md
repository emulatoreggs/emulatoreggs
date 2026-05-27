# Cxbx-Reloaded is an Xbox Emulator

## Cxbx-Reloaded Table of Contents

[TOC]

## Getting Started with Cxbx-Reloaded

### How to Install Cxbx-Reloaded
[Back to the Top](#cxbx-reloaded-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

Cxbx-Reloaded is available as a Windows executable file on Linux. This page will cover how to download and utilize the JAR file. 

To download Cxbx-Reloaded:

1. {{ umulauncher }}
2. Open the Cxbx-Reloaded download page, [https://cxbx-reloaded.co.uk/download](https://cxbx-reloaded.co.uk/download) on a browser of your choice
3. Download the latest version of Cxbx-Reloaded
4. Move the newly downloaded zip file to the `$HOME/Applications` folder and extract the zip file
    * {{ applications }}
5. Rename the newly extracted folder to `Cxbx-Reloaded`
6. In the `$HOME/Applications/Cxbx-Reloaded` folder, right click anywhere, click `Create New` > `Text File`
7. Name the text file `Cxbx-Reloaded.sh`
8. In the text file, write the following:

      #!/bin/sh
      umu-run WINEPREFIX=$HOME/Applications/CxbxReloaded/pfx GAMEID=umu-cxbxreloaded PROTONPATH=GE-Proton $HOME/Applications/CxbxReloaded/cxbx.exe

9. Save the text file and exit out of the text editor
10. Right click the newly created text file, {{ permissions }}
11. To run Cxbx-Reloaded.sh, double click `Cxbx-Reloaded.sh.sh`
    * The first launch may take a few minutes
12. Cxbx-Reloaded.sh will now be downloaded


## Cxbx-Reloaded Tips and Tricks
