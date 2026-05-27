# FreeJ2ME Plus is an J2ME emulator

## FreeJ2ME Plus Table of Contents

[TOC]

## Getting Started with FreeJ2ME Plus

### How to Install FreeJ2ME Plus
[Back to the Top](#freej2me-plus-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

FreeJ2ME Plus is available as a JAR file on Linux. This page will cover how to download and utilize the JAR file. 

To download FreeJ2ME Plus:

1. {{ java }}
2. Open the FreeJ2ME nightly page, [https://nightly.link/TASEmulators/freej2me-plus/workflows/ant/devel](https://nightly.link/TASEmulators/freej2me-plus/workflows/ant/devel) on a browser of your choice
3. Download the latest `freej2me-a530129.zip`  file by clicking the top-most link
4. Move the newly downloaded zip to the `$HOME/Applications` folder and extract the zip file
    * {{ applications }}
5. Rename the newly extracted folder to `freej2me`
6. In the `$HOME/Applications/freej2me` folder, right click anywhere, click `Create New` > `Text File`
7. Name the text file `FreeJ2ME-Plus.sh`
8. In the text file, write the following:

      #!/bin/sh
      cd "$HOME/Applications/freej2me"
      java -jar "$HOME/Applications/freej2me/freej2me.jar"

9. Save the text file and exit out of the text editor
10. Right click the newly created text file, {{ permissions }}
11. To run FreeJ2ME Plus, double click `FreeJ2ME-Plus.sh`
12. FreeJ2ME Plus will now be downloaded

## FreeJ2ME Plus Tips and Tricks
