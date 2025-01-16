---
title: Screen layout
layout: home
parent: Operating GaiaViz
nav_order: 1
---
## Overview - GUI Layout & Keyboard


The GUI is organized into 3 regions, the 3D scene, toolbar and console. There are several ways to interact via the standard keyboard and mouse, as well as optional hardware like the SpaceMouse & zSpace Stylus.

The left toolbar displays **mode** and **tool** indicators which you can click (or change mode with **scroll-wheel** or keyboard). It is worth noting that the devices operate **simultaneously**, ie: **Fly** the camera with the [**SpaceMouse**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#SpaceMouse) while modifying glyphs with the system [**mouse**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#mouse-trackball-trackpad--touchscreen) **AND** use the Keyboard ([**Game Mode**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#keyboard---game-mode) or [**Console**](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#text-tags--console)).

Important: At startup the keyboard is set to '**Game Mode**', where the '**Esc**' key will toggle fullscreen ON/OFF. However, you might **accidentally** find yourelf in one of the 3 different console modes ([Command Console](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#gui-command-console), [DB Menu](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#db-menu) or [Text Tag](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#text-tags--console)), in which case '**Esc**' will exit the console and return you back to 'Game Mode'.

---

## **Tool Bar**

### Headings and Coordinates

- The top box shows overall scene heading x degrees and cardinal direction.
- The second box down can shift between **Tilt** and **Roll**. Just click the box to change.
- The next three boxes show x, y, and z axes. Depending on which tool is selected, this can show coordinates, rotation, or scaling size. If in the Move or Combo tool, users can shift between **World** and **Local** coordinates by clicking on the top box, Heading.
    - Local coordinates show the location of the selected object on its parent's topology, and for the root node, its location on the parent grid.
    - World coordinates show the location of the selected object in relation to the primary grid. No matter what branch level the object is on, the world coordinates show where that object is in the overall scene.


Upper left : compass
upper right : FPS (frames per seconds=  performance)

Side bar :  mode display, tool list,

Bottom :  console feed back
- displays tools tips when you change tools
- displays id and tags when you select objects
- display the filepath when use save a screenshoot / load a file
- etc....

This is also where you will type in the console if needed.




GUI can be minimized or completely hidden with M key.