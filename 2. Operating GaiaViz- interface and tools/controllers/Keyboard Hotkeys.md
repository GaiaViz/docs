---
title: Keyboard
layout: home
parent: Keyboard and Mouse
nav_order: 1
---
Your keyboard controls the app like many 3D spatial software, nearly every key has a tools associated, and

The only exceptions are when you enter the Tag Mode ( hotkey `t` ) or the Console Mode ( hotkey `alt+enter` ). In those modes, you use the keyboard to type text
To exit those modes and return to normal controls, use the `esc` key.
## Keyboard - Game Mode


Note: Numbers, -, =, etc apply to the main keyboard, not the number pad.

A useful 'bug' is to change selection to another object (TAB, New, etc..) and do this while performing a rotation, it will continue to rotate, also applies to zoom and translate...

It is possible to press multiple keys at once (3-5 typical depending on the keyboard and key combo...) So for example, you can do a rotation and zoom while simultaneously changing the color.

### Global Settings

Here some hotkey that are good to know

| Hotkey | Fonction                                                                                                                                                                                |
| ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Esc    | **Fullscreen** Toggle and also exits console modes (return to **Game Mode**).                                                                                                           |
| M      | **Menu** display mode (**1, 3 or 40** text lines, toolbar **size** and **hide** GUI).                                                                                                   |
| B      | Background **Black/White**.                                                                                                                                                             |
| X      | **Lock axes** so that the **current tool** only effects: **X, Y, XY, XYZ**...<br>    - Hint: **Click** on the toolbar menu axes **[Coord (X/Y/Z): 0.0 ]** to toggle an axis **ON/OFF**. |

### Mouse Mode (Cam, Grid, Glyph)

The GUI indicator [mouse: (mode) ] determines what type of nodes are operated on by the (2D) mouse. To change the mode, click on the indicator or use the shortcut keys (when keyboard is in 'Game Mode'):


| Hotkey | Function                                    |
| ------ | ------------------------------------------- |
| C      | Camera mode, repeat to select next camera.  |
| G      | Grid mode, repeat to iterate through grids. |
| Tab    | Glyph mode, repeat to select next sibling.  |


*Note that **Shift+(mode key)** will select previous (of same node type).

**The 3D Mouse (ie: SpaceMouse) and zSpace Stylus have operation modes that are completely independent of the (2D) mouse mode.

### Camera Mode

| Hotkey    | Fonction                                                                                                             |
| --------- | -------------------------------------------------------------------------------------------------------------------- |
| C         | Enters 'Camera Mode' and next iterates through all cameras.<br>    (By default, the scene starts out with 4 cameras) |
| N         | creates a new camera object while in Camera mode                                                                     |
| **Alt+C** | reset camera position                                                                                                |
| Del       | removes a camera object while in this mode                                                                           |

{:  . important}
> *Hint: Creating new camera objects can be used to pre-set a journey through specific viewing angles of your viz.

### Grid Mode

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

### Create, Delete, Copy, Prune & Graft Glyphs

| Hotkey                 | Fonction                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| N                      | Creates a new node (based on the mode: Camera, Glyph, Grid...)<br>    - Use **Shift+N** when creating a Level 2 child node off the Level 1 root node.<br>    - Glyphs are type = 5.<br>    - In order to add glyphs to grids, go to Grid Mode, make sure the grid on which you want to add the node is **selected ON**, go back to Glyph Mode and then hit **N**. Alternatively, while still in Glyph Mode, you can use the arrow keys to move down branch levels, getting to branch level 0, the primary grid, and then paste the branches and children there.<br>    - A glyph with **parent_id=0** will be attached to the main grid. |
| Del                    | Delete node, deletes active node and all its child branches                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Ctrl+X**             | To cut (prune) and store the glyph tree or branch on the clipboard.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Shift+Ctrl+X**       | To cut (prune) to clipboard, with branch base in world coordinates.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Ctrl+C**             | To copy the glyph tree or branch to the clipboard.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Shift+Ctrl+C**       | To copy to clipboard, with branch base in world coordinates.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Ctrl+V**             | To paste (or graft) the clipboard to the active glyph (or Grid).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Ctrl+S**             | Saves all selected nodes with sub-branches (timestamped).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Shift+Ctrl+S**       | Saves just the selected nodes (without sub-branches).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Tool_Save Selected** | Saves entire branch(es) of selected nodes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 
### Traverse Forest & Trees

- **Left arrow** - select left sibling (SHIFT+arrow to skip towards first node)
- **Right arrow** - select right sibling (SHIFT skips towards last node)
- **Up arrow** - select child, up a branch level (SHIFT jumps to leaf)
- **Down arrow** - select parent, down a branch level (SHIFT jumps to root)