# GZDoom is an open source port of DooM.

## GZDoom Table of Contents

[TOC]

## Getting Started with GZDoom

### How to Install GZDoom
[Back to the Top](#gzdoom-table-of-contents)

??? info "The Basics"
    {{ home }} 

    {{ hiddenfolders }}
    
    {{ applications }}

To download GZDoom:

1. In Desktop Mode, open Konsole or a terminal of your choice
2. If you have not already added the Flathub user repo, type the following and press enter:
    * `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo --user`
3. Type the following and press enter:
    * `flatpak install org.zdoom.GZDoom --user -y`
4. Type the following two lines, one at a time, and press enter after each line:
    * `flatpak override org.zdoom.GZDoom --filesystem=host --user`
    * `flatpak override org.zdoom.GZDoom --share=network --user`

If you have Discover installed, you may also use Discover to install Dolphin. Make sure you have the Flathub repo added (Step 2 in the section above). 

### How to Install DooM Mods

[https://github.com/MrMendelli/DOOM-Scripts](https://github.com/MrMendelli/DOOM-Scripts)