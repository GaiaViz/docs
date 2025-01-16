---
title: Modes
layout: home
nav_order: 3
parent: Operating GaiaViz
---
# Modes

GaiaViz has different modes that you select via the keyboard: camera (C key) explore the scene
- glyph : edit the glyphs
- grids, to work on the grids
- tag mode, to annotate the scene
- console mode,
### Mouse Mode (Cam, Grid, Glyph)

The GUI indicator [mouse: (mode) ] determines what type of nodes are operated on by the (2D) mouse. To change the mode, click on the indicator or use the shortcut keys (when keyboard is in 'Game Mode'):


| Hotkey | Function                                    |
| ------ | ------------------------------------------- |
| C      | Camera mode, repeat to select next camera.  |
| G      | Grid mode, repeat to iterate through grids. |
| Tab    | Glyph mode, repeat to select next sibling.  |
*Note that **Shift+(mode key)** will select previous (of same node type).

**The 3D Mouse (ie: SpaceMouse) and zSpace Stylus have operation modes that are completely independent of the (2D) mouse mode.



## Camera mode 

The camera mode lets you move around the scene without modifying it. It allows you to fly through the scene, select an object to inspect closer


There are several cameras, that select one after the other,

Each camera have its specific settings, like the background color, the tags display style, as well as the position. You can have several cam and each camera has specific settings, like the background color / image / video stream.

You can freeze a camera to keep an specific point of view.

{: .important}
> Tips
> 
> If you get lost in the scene, delete your current camera to get back to the default center position.


| Hotkey    | Fonction                                                                                                             |
| --------- | -------------------------------------------------------------------------------------------------------------------- |
| C         | Enters 'Camera Mode' and next iterates through all cameras.<br>    (By default, the scene starts out with 4 cameras) |
| N         | creates a new camera object while in Camera mode                                                                     |
| **Alt+C** | reset camera position                                                                                                |
| Del       | removes a camera object while in this mode                                                                           |

{:  . important}
> *Hint: Creating new camera objects can be used to pre-set a journey through specific viewing angles of your viz.

## Glyph, Grid and Tag modes

To add, delete, layers, style, size grid.

## Grid mode

The grids are the base planes where all objects are attached.

You can change the color overlay, the color of their lines, their texture (image or video)

| Hotkey    | Fonction                                                                                                   |
| --------- | ---------------------------------------------------------------------------------------------------------- |
| G         | Enters 'Grid Mode' and next iterates through all grids.                                                    |
| **ALT-G** | toggles an object between **Glyph** and **Grid** types                                                     |
| **N**     | Will create a new grid (when 'mouse: grid' mode is active) as a child of the current node (glyph or grid). |
- **`branch_level`** = 0 for ALL grids, Hence, any (root) glyphs directly attached will start at level = 1.
- Grids are node **`type = 6, np_topo_id = 8`** (plane) with **`np_geometry_id = 21`** (square).
- Scaling the grid compacts the spacing (translation) of attached (root) nodes but does NOT affect their size, and is axis specific.
    - eg. Scale the Z-axis of the grid to compact or expand a vertical stack of (root level) glyphs.
- To move grids, see [Move, Rotate or Scale Objects](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#move-rotate-or-scale-objects).
- To change color, texture, or transparency, see [Texture, Color & Transparency](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#texture-color--transparency).
- To change grid unit size and segment count see [Toplogy & Geometry](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#topology--geometry)
    - Hint: Segments = 1 is an empty rectangle, (no grid lines).

## Tag mode

The tag mode allows to edit the tags, to annotate and Press `T` to enter the tag mode, `f` to cycle the font

## Console mode `alt+enter`

The console mode allows for finer selection, for examples by branch level or color.

| Hotkey      | Function               |
| ----------- | ---------------------- |
| alt + enter | Enter the console mode |
| "help"      | shows the console help |
| Esc         | Exit                   |
|             |                        |

