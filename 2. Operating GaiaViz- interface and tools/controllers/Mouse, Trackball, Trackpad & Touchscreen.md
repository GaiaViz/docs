---
title: Mouse
layout: home
parent: Keyboard and Mouse
nav_order: 2
---

## Mouse, Trackball, Trackpad & Touchscreen


Behavior is based on the active **[mouse: (mode) ]** and **[tool: (type) ]**.

- **Mouse Wheel** - changes tool type.
- **L-Click** on **[mouse: (mode) ]** indicator will switch between **Camera**, **Grid** & **Glyph** mode.
- **L-Click** on any of menubar tool to set the **[tool: (type) ]**.

### Mouse Navigation

- **L - Hold** on scene background to **XY ORBIT** around current object.
- **L+R - Hold** on background to **XZ ORBIT** circle and **ZOOM** in/out.
- **Mouse scroll** - Camera zooms in/ out with 2D mouse scroll wheel (when in Camera Orbit active).
- **R - Hold** on background to **FLY** camera around scene.
- **Hints:**
    - Directly switch between camera orbit XY and XZ modes by using **L-Hold** while pressing (or releasing) **R-Hold**.
    - After using **FLY** mode (**R-Hold**) you will then be able to use **LOOK** mode using **L-Hold**.

### Mouse Selection

It is possible to **L/R-Click** to select using several of the tools (Combo, Move, Scale, etc.) However other tools use the clicks to change the glyph attributes (topo, color, etc.)

- With **[tool: Select]** you can create a selection set:
    - **L-Click** on an object will select it (can select multiple).
    - **R-Click** on object de-selects it.
    - **L-Hold** to drag a selection box (add to selection).
    - **R-Hold** to drag a de-selection box (removes objects).

### Mouse Tools



Create
    - **L-Click** on background creates a new hyperglyph (pin with torus).
    - **L-Click** on a glyph creates a new (attached) child glyph. (Note: if you wish to create a child node off of a root node, you will need to hold **Shift L-Click**.)
    - **R-Click** deletes glyph.
Link
    - **L-Click** on the 'A' link end and then select the 'B' link end.
    - **R-Click** cancels and resets for picking the 'A' link end.
    - Note: You can only connect root nodes to other root nodes.
Combo
    - **L-Hold** drags selected objects in XY (L-R & Forward-Back).
    - **R-Hold** scale objects up/down, and increases/decreases ratio.


Move
    - **L-Hold** moves objects in XY (L-R & Forward-Back).
    - **R-Hold** moves objects in XZ (L-R & Up-Down).


Rotate
    - **L-Hold** rotates objects on X & Y axes (Heading, Tilt).
    - **R-Hold** rotates objects on Z axes (Roll)
- 
- **[Size]**
    - **L-Click** to increase/decrease scale.
    - **R-Click** to increase/decrease ratio.
- 
- **[Topo], [Geometry], [Color], [Texture]**
    - **L-Click** for next (topo type, index color, texture map, etc...).
    - **R-Click** for previous type.

- **[Hide]**
    - **R-Click** to Hide all sub-branches of selected node.
    - **L-Click** to un-Hide sub-branches.
    - See **Keyboard Game Mode** commands below for hiding per branch level, etc.

- **[Tag]**
    - **L-Click** to select a glyph, and then use keyboard to modify or enter a new tag.
        - Repeating **L-Click** on the same glyph will change it's draw style (color, outline).
    - **R-Click** will hide the tag (but the text will be retained).
    - **Enter** will alternate between **Tag Edit** mode and **Tag Style** mode (tag game mode).
        - See **Text Tag Console** section for details on tag formatting (including URL's).




- **Hidden Tools - accessible via scrollwheel**
    - **[Alpha]** - Changes glyph opacity (transparency).
    - **[Channel]** - Animation channel (subscribes selected nodes to tracks).
    - **[Freeze]** - Freezes animation and editing.
    - **[Set High]** - Restricts the max position of a glyph to current location.
    - **[Set Low]** - Restricts the minimum position (is specific to active axes **X** key).

Hint: The console will display tips on tool usage when you switch to a new tool.

---