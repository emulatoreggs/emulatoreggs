# openDoJa is a reimplementation of the DoJa 5.1 runtime and related APIs.

## openDoJa Table of Contents

[TOC]

## Getting Started with openDoJa

### How to Install openDoJa
[Back to the Top](#opendoja-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

openDoJa is available as a JAR file on Linux. This page will cover how to download and utilize the JAR file. 

To download openDoJa:

1. {{ java }}
2. Open the openDoJa releases page, [https://github.com/GrenderG/openDoJa/releases](https://github.com/GrenderG/openDoJa/releases) on a browser of your choice
3. Download the latest `opendoja-release.jar` file
4. Move the newly downloaded JAR file to the `$HOME/Applications` folder
    * {{ applications }}
5. In the `$HOME/Applications` folder, right click anywhere, click `Create New` > `Text File`
6. Name the text file `openDoJa.sh`
7. In the text file, write the following:

      #!/bin/sh
      java -jar "$HOME/Applications/opendoja-release.jar"

8. Save the text file and exit out of the text editor
9. Right click the newly created text file, {{ permissions }}
10. To run openDoJa, double click `openDoJa.sh`
11. openDoJa will now be downloaded

## openDoJa Tips and Tricks