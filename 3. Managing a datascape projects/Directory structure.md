---
title: Directory structure
layout: home
nav_order: 2
parent: Managing Datascape Projects
---
# How GaiaViz stores data: folder structure

GaiaViz stores the data as Comma Separated Values formatted plain text files in a *datascape*. A datascape is a folder on your local file system, including any subfolders.

Because files are plain text files, you can use other text editors, spreadsheets editor and file managers to edit and manage files.

You can create a datascape anywhere your operating system allows, but we do recommend using our structure to keep things organized.

You can open multiple datascapes as individual windows, or within the same scene, although tags merging is not yet supported.

```
.
├── Docs
│   ├── doxy
│   ├── hardware
│   └── web
├── OSC
│   ├── GaiaViz-Remote-v1.tosc
│   └── GaiaViz-Remote-v1_install.txt
├── User
│   ├── _Global_
│   │   ├── av
│   │   ├── csv
│   │   ├── gui
│   │   ├── images
│   │   ├── json
│   │   ├── models
│   │   └── plugins
│   ├── FileViz
│   │   ├── yyyy-mm-dd
│   │   │   ├── FileViz
│   ├── ImageViz
│   ├── Your-user-name
│ 	│   ├── Your project A
│ 	│   ├── Your project B
│ 	│   │   ├── Project B-v1
│ 	│   │   ├── Project B-v2
│ 	│   │   └── Project B-v3
│ 	│   └── Your project C
│   └── Prototypes
```


![]({% link /assets/images/Datascape-ProjectFile.jpg %})