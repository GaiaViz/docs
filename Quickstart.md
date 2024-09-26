---
title: Quickstart
nav_order: 2
layout: home
---

GaiaViz is quick to try out, just download the zip file, extract it on a windows machine and run the gaiaviz.exe app from its folder. If you wish to try the remote capacities, allow network communication when prompted. The app is ready with 3 presets, accessible via key 1, 2, and 3.

1. Download GaiaViz.zip from our site :
2. Extract the content and run the app from its folder.
3. If you wich to connect a [Edge AI] or [GaiaRemote], allow the network communication dialog.
4. Explore the demos by pressing 'L' and choosing

Navigate with a mouse, even better, a spacemouse.
Use the tools with the keyboard.

# Quickstart
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}



4. 
# Requirements & prerequisites

## Prerequisite:
- Navigation is pretty straight forward
- GaiaViz operators needs to be familiar with 3D tools and data wrangling process.

The minimum requirements for GaiaViz are:

| Hardware    | Operating system               | Memory:                                                                    |
| ----------- | ------------------------------ | -------------------------------------------------------------------------- |
| Hardware    | Dedicated GPU                  |                                                                            |
| OS          | windows app + DLL              | *Non-official macOS using whiskey bottles<br>, a PC game emulator for mac* |
| RAM :       | 8Go available                  |                                                                            |
| Disk space: | adapted to your dataset volume |                                                                            |

> [!INFO] 
> Depending on your use-case, the required memory may vary


- Data wrangling tools: Spyder environment / Anaconda 
- nVidia drivers
- live video 
- sql connection: a MySQL database 



## Hardware

memory: as big as the dataset you wish to work with
dedicated GPU (the bigger GPU, the bigger dataset can be loaded


## Software

Operating System: MS Windows 7, 10, 11
GaiaViz also needs some the following dll that sometime.
This dll is provided in the .zip folder.

System Requirements
1. Operating system: Windows 10+ 
2. RAM : 8Go available for
3. Disk space: sufficient for your dataset volume
-------------------------


# Install, update, uninstall GaiaViz

## Install
1. Download the app from gaiviz.com and extract it. You can launch GaiaViz from this folder.
2. If needed, install the .dll provided with the package

## Update 

1. Back-up the "User" folder
2. Download the new version and extract it
3. Replace the default "User" folder with your own


*GaiaViz app maintains backward compatibility and can handle files created with/for a previous version. On first open, it adapt the datascape's files to the new format. This operation might render the files unopenable to previous version, so please do back-up your data before upgrading.


## Uninstall
If you need to uninstall GaiaViz, simply delete the folder.


# Configuration

Global files
- GitHub viz
- Presets
- OSC ports (+ remotes, find them)
- projects files structure

Network access Permissions for OSC

To use some of GaiaViz features, you'll need to give it Network Access authorization from the pop-up dialog.

When GaiaViz launches for the first time, or when you configure the OSC ports the first time, windows will automatically present you the dialog box.

## OSC (Open Sound Control)
- OSC port and IP config is stored in the globals table ('User/_Global_/csv/np_globals.csv')