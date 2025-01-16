---
title: System Requirements
nav_order: 1
layout: home
parent: Getting started
---

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

# Requirements & prerequisites

## Prerequisite:

- Navigation is pretty straight forward
- GaiaViz operators needs to be familiar with 3D tools and data wrangling process.

The minimum requirements for GaiaViz are:

| Item        | Requirements                   | Notes                                                                      |
| ----------- | ------------------------------ | -------------------------------------------------------------------------- |
| Hardware    | Dedicated GPU                  |                                                                            |
| OS          | windows app + DLL              | *Non-official macOS using whiskey bottles<br>, a PC game emulator for mac* |
| RAM :       | 8Go available                  |                                                                            |
| Disk space: | adapted to your dataset volume |                                                                            |

{: .info }
> Depending on your use-case, the required memory may vary


- Data wrangling tools: Spyder environment / Anaconda 
- nVidia drivers
- live video

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

If you wish to stream data over OSC or to remotely control GaiaViz using, please refer to this page for further details on the topic : [[OSC (Open Sound Control)]]