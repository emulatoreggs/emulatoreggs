# Java

This page will cover how to download and utilize Java.

## Java Tips and Tricks Table of Contents

[TOC]

***

## How To Install Java
[Back to the Top](#java-tips-and-tricks-table-of-contents)

1. In the `$HOME/Applications` folder, create a `jdk` folder :material-information-outline:{ title="{{ steamdeckdesktopmode }}" }
    * {{ applications }}
2. Open the Java JDK website, [https://jdk.java.net/](https://jdk.java.net/) on a browser of your choice 
3. Click `JDK ##` to the right of `Ready for Use` 
    * The ## refers to the version number, this may vary depending on when you are downloading Java
4. Download the `tar.gz` file to the right of `Linux / x64` to the newly created `$HOME/Applications/jdk` folder
5.  Right click `openjdk-##.#.#_linux-x64_bin.tar.gz`, click `Extract > Extract Archive here`
    * If it creates a subfolder, move the contents directly to `$HOME/Applications/jdk`
6.  In the `$HOME` folder, right click the `.bashrc` file, click `Open with Kate` or a text editor of your choice
    * `$HOME/.bashrc` is a hidden file by default. In Dolphin (file manager), click the hamburger menu in the top right, click `Show Hidden Files` to see these files
7.  At the bottom of the `.bashrc` file, paste the following two lines:

      export JAVA_HOME=$HOME/Applications/jdk
      export PATH=$JAVA_HOME/bin:$PATH

8.  Save and exit out of the `.bashrc` file
9.  Java will now be installed
    * If you had any terminals open previously, close these out and re-open them in order to use Java through the command-line

To update JDK, replace the files in `$HOME/Applications/jdk` with the latest files from [https://jdk.java.net/](https://jdk.java.net/).

## How to Utilize Java with Applications

Make sure you have downloaded and installed Java following the steps in the [How To Install Java](#how-to-install-java) section prior to reading this section.

1. Open Kate or a file editor of your choice
2. At the top of the file, write the following line:
    * `#!/bin/bash`
3. Press enter and use the following format:
    * `java -jar /PATH/TO/APPLICATION.JAR`
4. Save the text file using the following format:
    * `APPLICATIONNAME.SH`
5. Right click the newly created text file, {{ permissions }}
6. To run the application, double click `APPLICATIONNAME.SH`

