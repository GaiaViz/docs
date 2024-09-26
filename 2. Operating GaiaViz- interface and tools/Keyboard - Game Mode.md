---
title: Keyboard
layout: home
parent: Interface and tools
---

## Keyboard - Game Mode


Note: Numbers, -, =, etc apply to the main keyboard, not the number pad.

A useful 'bug' is to change selection to another object (TAB, New, etc..) and do this while performing a rotation, it will continue to rotate, also applies to zoom and translate...

It is possible to press multiple keys at once (3-5 typical depending on the keyboard and key combo...) So for example, you can do a rotation and zoom while simultaneously changing the color.

### Global Settings

- **ESC** - **Fullscreen** Toggle and also exits console modes (return to **Game Mode**).
- **M** - **Menu** display mode (**1, 3 or 40** text lines, toolbar **size** and **hide** GUI).
- **B** - Background **Black/White**.
- **X** - **Lock axes** so that the **current tool** only effects: **X, Y, XY, XYZ**...
    - Hint: **Click** on the toolbar menu axes **[Coord (X/Y/Z): 0.0 ]** to toggle an axis **ON/OFF**.

### Mouse Mode (Cam, Grid, Glyph)

The GUI indicator [mouse: (mode) ] determines what type of nodes are operated on by the (2D) mouse. To change the mode, click on the indicator or use the shortcut keys (when keyboard is in 'Game Mode'):

- **C** - Camera mode, repeat to select next camera.
- **G** - Grid mode, repeat to iterate through grids.
- **Tab** - Glyph mode, repeat to select next sibling.

*Note that **Shift+(mode key)** will select previous (of same node type).

**The 3D Mouse (ie: SpaceMouse) and zSpace Stylus have operation modes that are completely independent of the (2D) mouse mode.

### Camera Mode

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#camera-mode)

- **C** - Switches to 'Camera Mode' and iterates through all cameras.
    - By default, the scene starts out with 4 cameras.
    - **Alt+C** - reset camera position.
- **N** creates a new camera object while in Camera mode.
- **Del** removes a camera object while in this mode.

*Hint: Creating new camera objects can be used to pre-set a journey through specific viewing angles of your viz.

### Grid Mode

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#grid-mode)

- **G** - Switches to 'Grid Mode' and iterates through all grids.
- **ALT-G** - toggles an object between **Glyph** and **Grid** types.
- **N** - Will create a new grid (when 'mouse: grid' mode is active) as a child of the current node (glyph or grid).
- **`branch_level`** = 0 for ALL grids, Hence, any (root) glyphs directly attached will start at level = 1.
- Grids are node **`type = 6, np_topo_id = 8`** (plane) with **`np_geometry_id = 21`** (square).
- Scaling the grid compacts the spacing (translation) of attached (root) nodes but does NOT affect their size, and is axis specific.
    - eg. Scale the Z-axis of the grid to compact or expand a vertical stack of (root level) glyphs.
- To move grids, see [Move, Rotate or Scale Objects](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#move-rotate-or-scale-objects).
- To change color, texture, or transparency, see [Texture, Color & Transparency](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#texture-color--transparency).
- To change grid unit size and segment count see [Toplogy & Geometry](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#topology--geometry)
    - Hint: Segments = 1 is an empty rectangle, (no grid lines).

### Create, Delete, Copy, Prune & Graft Glyphs


- **N** - Creates a new node (based on the mode: Camera, Glyph, Grid...)
    - Use **Shift+N** when creating a Level 2 child node off the Level 1 root node.
    - Glyphs are type = 5.
    - In order to add glyphs to grids, go to Grid Mode, make sure the grid on which you want to add the node is **selected ON**, go back to Glyph Mode and then hit **N**. Alternatively, while still in Glyph Mode, you can use the arrow keys to move down branch levels, getting to branch level 0, the primary grid, and then paste the branches and children there.
    - A glyph with **parent_id=0** will be attached to the main grid.
- **Del** - Delete node, deletes active node and all its child branches
- **Ctrl+X** - To cut (prune) and store the glyph tree or branch on the clipboard.
    - **Shift+Ctrl+X** - To cut (prune) to clipboard, with branch base in world coordinates.
- **Ctrl+C** - To copy the glyph tree or branch to the clipboard.
    - **Shift+Ctrl+C** - To copy to clipboard, with branch base in world coordinates.
- **Ctrl+V** - To paste (or graft) the clipboard to the active glyph (or Grid).
- **Ctrl+S** - Saves all selected nodes with sub-branches (timestamped).
    - **Shift+Ctrl+S** - Saves just the selected nodes (without sub-branches).
    - **Tool_Save Selected** - Saves entire branch(es) of selected nodes.

### Traverse Forest & Trees

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#traverse-forest--trees)

- **Left arrow** - select left sibling (SHIFT+arrow to skip towards first node)
- **Right arrow** - select right sibling (SHIFT skips towards last node)
- **Up arrow** - select child, up a branch level (SHIFT jumps to leaf)
- **Down arrow** - select parent, down a branch level (SHIFT jumps to root)

### Select, Hide & Freeze

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#select-hide--freeze)

- **Spacebar** - toggles the wireframe that indicates a node is selected **ON/OFF**.
    - **Alt+Spacebar** - toggles current node selection **ON/OFF**.
- **H** - Hides the object, but it will continue to (invisibly) animate.
    - **Shift+H** to unhide all nodes.
    - **Alt+H** to hide nodes by increasing branch level.
    - **Shift+Alt+H** to hide nodes by decreasing branch level.
- **F** - Freeze will stop the object's movement and lock editing it.
- **`** (left single quote) - **Default** behavior is to toggle **Select ALL/NONE** glyphs.
    - **Alt+`** will invert the selection (*future feature).
- **'** & **Shift+'** (right single quote) - will either move up or down (with Shift) a branch level from the selected node and select all nodes at that new branch level on that particular glyph.
- **Ctrl+A** - Also toggles select **ALL ON/OFF**.
- **Alt+~** - Inverses selection set.

### Subsample

[](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#subsample)

- **\** (backslash) - Subsamples nodes to draw faster
    - **Shift+\** - Reverses subsampling
    - Reduces number of root nodes by half with each **\**.
- **Alt+\** and **Shift+Alt+\** specifies the **branch_level** to apply sub-sampling, (default is **branch_level** = 1).

### Move, Rotate or Scale Objects


- **R** - Rate mode can be either **keydown** or **increment**.
    
    - **rate mode: keydown** - (default) will apply the rate while holding down the key.
    - **rate mode: increment** - will increment the rate with each press (including key repeat).
        - Hint: you can reset the rate to zero by switching to **keydown** mode and tapping the same key.
- #### Move (WASD + QE)
    
- - **D** - increase X position (translate)
    - **A** - decrease X
    - **W** - increase Y
    - **S** - decrease Y
    - **E** - increase Z
    - **Q** - decrease Z
- #### Rotate (same as Move with **Alt** key)

- - **Alt+D** - Right (rotate about Y axis)
    - **Alt+A** - Left
    - **Alt+W** - Up (X axis)
    - **Alt+S** - Down
    - **Alt+E** - CW (Z axis)
    - **Alt+Q** - CCW
- **Z** - Scale objects up (**Shift+Z** for down).
    
    - **Alt+Z** - Spreads (translates) sub-grid child nodes (must be in **Grid** mode).
    - Applies ONLY to active axes (**X** key).
- **I** - Increases inner radius of **torus** geo, **rod** topo or **link** node, (**Shift+I** decreases).
    

### Translate Position Limits



- Set Points restrict the translate_x/y/z range of an object.
    - `[` (L bracket) - Low set point, object default is z = 0.0 for ground level.
    - `]` (R bracket) - High set point, set points are specific to active (**X*** key) axes.

### Topology & Geometry


- **J** - Next '**topo**' type, **Shift+J** for previous topo.
    - **ALT+J** will change which parent facet (on a cube...).
- **O** - Object geometry, does not change the 'topo' type.
    - **ALT-O** if using an imported 3D object file, use this command to keep this imported geometry and rotate through topologies. Coming in next release later in Feb 2021.
- **ALT+G** - Set current glyph node to be a grid (topo and geometry).
- **Y** - Increases the (Grid) **`segment_x y z`** count (**Shift+Y** - decreases the count)
    - Z (**`segment_z`**) is stacks of grids as 3D layers.
    - Hint: If X & Y segments = 1, the grid is an empty rectangle.
    - Actions ONLY apply to the **active axes** (**X** key) component(s).
    - **ALT+Y** - increase unit size spacing (**Shift+Alt+Y** to decrease).
        - **`np_node`** table stores (grid) spacing (`**np_node**` table: **`auxa_x y z`**).
    - Total grid dimensions are determined by the grid **spacing X segments = length** (per axis).

### Texture, Color & Transparency

- **Texture Settings**
    - **V** - Video or image Texture map (**Shift+V** for previous).
    - **Alt+V** - increase wireframe thickness (**Shift+Alt+V** to decrease).
        - *Wireframe thickness does not work in VMware.
    - Images are loaded from 'User/_Global_/images' folder.
        - **texture_id** corresponds to the (alpha-numeric) order of loading.
- **Object Color Settings**
    - **=** (equal) - next (palette) index color.
        - **Alt+'='** - next color palette.
    - **-** (minus) - previous index color.
        - **Alt+'-'** - previous color palette.
- **Transparency Settings**
    - **9** - Less opaque (more transparent).
    - **0** - More opaque.
- **Alternate Color (grid lines)**
    - **Alt+9** - decrease opacity of the grid lines.
    - **Alt+0** - increase opacity of grid lines.
    - **Shift+Alt+9** - prev color ID of grid lines.
    - **Shift+Alt+0** - next color ID of grid lines.
- **Global Color Settings**
    - **B** - Background color, toggle between black and white
    - **8** - Transparency mode (subtractive, additive, dark, none)

### Animation - Channels & Tracks


- **P** - Plays track animation ([dataset]_np_ch-tracks.csv & [dataset]_np_ch-map.csv)
    - Press **P** again to pause/play.
    - **'>'** (comma) - Increase playback speed.
    - **'<'** (period) - Decrease playback speed (negative values play in reverse).
- **Alt + '>'** (comma) - Channel Up for selected nodes.
- **Alt + '<'** (period) - Channel Down for selected nodes.

### Browser URL & record_id Retrieval

- **U** - Opens Tag title URL in the system browser, supports HTML href="...".
    - If no URL in title, then uses default URL with record_id appended.
    - Can also open applications and files based on OS default mime type.
    - ALSO... launches URL as tag title ie: [http://example.com](http://example.com) or app.exe
