---
title: Modes and tools
layout: home
nav_order: 1
parent: Interface and tools
---
# Modes

GaiaViz has different modes that you. You can either change 

## Camera mode 

you can have several cam and each camera has specific settings, like the background color / image / video stream,

## Glyph, Grid and Tag modes

To add, delete, layers, style, size grid.

A grid create 


The tag mode allows Press `T` to enter the tag mode, `f` to cycle the font

## Console mode `alt+enter`

The console mode allows for finer selection, for examples by branch level or color.
Enter the console mode by pressing the  key combinaison.

# Tools

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



## SpaceMouse

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

## zSpace Stylus


**zSpace system** AR/VR computers are **XR devices** that include a **6DOF stylus** (aka: **zStylus**).

- The **[zStylus: (tool) ]** GUI indicator is visible **ONLY** when a [zSpace System](https://github.com/GaiaViz/GaiaViz/wiki/zSpace) is used.
- **zStylus** tool operates independently of other input devices (keyboard, mouse...).
    - Most tools are similar to standard mouse tools described above.
        - **Center Button** - is equivalent to mouse **L-Click**.
        - **Right Button** - is equivalent to **R-Click**.
        - **Left Button** - changes tool type.


[[GUI Consoles]]
