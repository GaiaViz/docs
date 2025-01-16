---
title: Move, Rotate or Scale Objects
layout: home
nav_order: 2
parent: Tools
---
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
