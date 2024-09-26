---
title: Tools
layout: home
parent: Interface and tools
nav_order: 2
---

## Overview - GUI Layout & Keyboard

This page is an overview of all User Commands (tools, modes, console(s), etc.)

- Additional **detailed usage** is here: [**Tools**](https://github.com/GaiaViz/GaiaViz/wiki/Tools) or [**Text Consoles**](https://github.com/GaiaViz/GaiaViz/wiki/Text-Consoles).

The GUI is organized into 3 regions, the 3D scene, toolbar and console. There are several ways to interact via the standard keyboard and mouse, as well as optional hardware like the SpaceMouse & zSpace Stylus. The left toolbar displays **mode** and **tool** indicators which you can click (or change mode with **scroll-wheel** or keyboard). It is worth noting that the devices operate **simultaneously**, ie: **Fly** the camera with the [**SpaceMouse**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#SpaceMouse) while modifying glyphs with the system [**mouse**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#mouse-trackball-trackpad--touchscreen) **AND** use the Keyboard ([**Game Mode**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#keyboard---game-mode) or [**Console**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#text-tags--console)).

Important: At startup the keyboard is set to '**Game Mode**', where the '**Esc**' key will toggle fullscreen ON/OFF. However, you might **accidentally** find yourelf in one of the 3 different console modes ([Command Console](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#gui-command-console), [DB Menu](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#db-menu) or [Text Tag](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#text-tags--console)), in which case '**Esc**' will exit the console and return you back to 'Game Mode'.

---

## **Tool Bar**

### Headings and Coordinates

- The top box shows overall scene heading x degrees and cardinal direction.
- The second box down can shift between **Tilt** and **Roll**. Just click the box to change.
- The next three boxes show x, y, and z axes. Depending on which tool is selected, this can show coordinates, rotation, or scaling size. If in the Move or Combo tool, users can shift between **World** and **Local** coordinates by clicking on the top box, Heading.
    - Local coordinates show the location of the selected object on its parent's topology, and for the root node, its location on the parent grid.
    - World coordinates show the location of the selected object in relation to the primary grid. No matter what branch level the object is on, the world coordinates show where that object is in the overall scene.



## [SpaceMouse](https://github.com/GaiaViz/GaiaViz/wiki/3D-Mouse#spacemouse)


The **3Dconnexion SpaceMouse** (family) are 6DOF devices that operate the camera and modify glyphs (currently selected by the keyboard, system mouse/trackpad/touchscreen or zSpace Stylus).

- The **[3Dmouse: (tool) ]** GUI indicator is visible (**ONLY**) when a [3Dconnexion driver is installed](https://github.com/GaiaViz/GaiaViz/wiki/3D-Mouse#spacemouse).
- **L button** - changes mode between **Camera** (**blue**) and **Glyph** (**red**).
- **R button** - changes **tool** type:
    - Camera mode (**blue**) has two navigation methods:
        - **[Orbit]** - around (**Twist/Tilt**) and zoom in/out (**Forward/Back**) of currently selected object.
        - **[Fly]** - around the scene (6DOF).
    - Glyph mode (**red**) has several tools:
        - **[Combo]** - orientation (**Twist/Tilt/Roll**) and translate (**Push XYZ**).
        - **[Move]** - translate (**Push XYZ**).
        - **[Rotate]** - orientation (**Twist/Tilt/Roll**).
        - **[Size]** - Uniform scale (**Up/Down**), non-uniform (**Left/Right**) & (**Forward/Back**).
        - **[Color]** - **Alpha** (**Up/Down**) or **RGB** color (**Twist/Tilt/Roll**).

Hint: can also **L/R-click** on GUI indicator to change modes with (2D) mouse or zSpace Stylus.

**Important**, you may need to [disable the 3D connexion GUI overlay](https://github.com/GaiaViz/GaiaViz/wiki/Space-Mouse) to prevent popping up on top of the app.

---

## [zSpace Stylus](https://github.com/GaiaViz/GaiaViz/wiki/zSpace)


**zSpace system** AR/VR computers are **XR devices** that include a **6DOF stylus** (aka: **zStylus**).

- The **[zStylus: (tool) ]** GUI indicator is visible **ONLY** when a [zSpace System](https://github.com/GaiaViz/GaiaViz/wiki/zSpace) is used.
- **zStylus** tool operates independently of other input devices (keyboard, mouse...).
    - Most tools are similar to standard mouse tools described above.
        - **Center Button** - is equivalent to mouse **L-Click**.
        - **Right Button** - is equivalent to **R-Click**.
        - **Left Button** - changes tool type.


[[GUI Consoles]]

## [(OS) Command Line Flags](https://github.com/GaiaViz/GaiaViz/wiki/System-Console)

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#os-command-line-flags)

The app excepts command line arguments:

- For usage: `C:\>data\GaiaViz.exe -?`
- To load a dataset:
    - `-d [path] [file filter]` to load entire dataset:
        - `C:\>data\GaiaViz -d usr\GaiaViz\ *.*`
    - `-f` to load specific file(s):
        - `C:\>data\GaiaViz -f User\[dataset]\csv\[dataset]_np_node.csv -f "usr\other image.jpg"`
            - Note that double quotes are needed (only) for file paths that have spaces.
- Launch GaiaViz dataset using the auto-generated .BAT file:
    - `C:\>data\GaiaViz\User\Edge-AI\2023-08-31\Edge-AI_v3_npe.bat`
    - You can of course create your own .BAT files:
        - The specificed data path is relative to the location of the batch file.
        - MSW batch files require the path only use the backslash (vs POSIX forward slash).
            - Note that as of W7, a forward or backslash works for almost everything (else).

*KNOWN BUG (issue #298) prevents loading node CSV tables.