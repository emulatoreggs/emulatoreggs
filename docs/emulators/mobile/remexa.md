# ReMEXA is a modern Java reimplementation and host runtime for SoftBank MEXA S-Appli, Vodafone V-Appli, and J-SKY V-Appli software.

## ReMEXA Table of Contents

[TOC]

## Getting Started with ReMEXA

### How to Install ReMEXA
[Back to the Top](#remexa-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

ReMEXA is available as a JAR file on Linux. This page will cover how to download and utilize the JAR file. 

To download ReMEXA:

1. {{ java }}
2. Open the ReMEXA releases page, [https://github.com/Yuvi-App/ReMEXA/releases](https://github.com/Yuvi-App/ReMEXA/releases) on a browser of your choice
3. Download the latest `ReMEXA-Release.jar`  file
4. Move the newly downloaded JAR file to the `$HOME/Applications` folder
    * {{ applications }}
5. In the `$HOME/Applications` folder, right click anywhere, click `Create New` > `Text File`
6. Name the text file `ReMEXA.sh`
7. In the text file, write the following:

      #!/bin/sh
      java -jar "$HOME/Applications/ReMEXA-Release.jar"

8. Save the text file and exit out of the text editor
9. Right click the newly created text file, {{ permissions }}
10. To run ReMEXA, double click `ReMEXA.sh`
11. ReMEXA will now be downloaded

## ReMEXA Tips and Tricks