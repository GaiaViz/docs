---
title: GUI consoles
layout: home
parent: Operating GaiaViz
---


### Keyboard - Game Mode Console

- Outputs user actions and system messages (status, warn, err...)
    - **M** - key will switch the number of lines shown (or hide completely).
    - Keyboard Game Mode actions are described above.

### (GUI) Command Console

- **Enter** key - Enters Command Console (from Game Mode).
- Type '**?**' and press **Enter** for command usage '**help**'.
- **Esc** key - leave Command Console and return keyboard to **Game Mode**.

### Text Tag Console

- **T** - Toggles the **Tag Tool** ON/OFF.
    - **Enter** - switches between **Tag Edit** and **Tag Style**:
        - **Tag Edit** mode modifies the text.
            - Press **Enter** or **Esc** to return to **Tag Style** mode.
        - **Tag Style** keys:
            - Can select tags as usual with keyboard keys and/or mouse.
            - **H** - toggles hide/unhide.
                - **Alt+H** - hide all text tags.
            - **F** - changes the font type (**Shift+F** for previous).
            - **Z** - scales the tag size up (**Shift+Z** scales down).
            - **B** - changes the tag box style (outline or node color text).


- Camera mode (**C** key) controls scene wide tag view behavior:
    - **Z** - scales display size of all tags.
    - **Alt+Z** - changes all (visible) tags view mode, as follows:
        - **Hide All** mode '0' (does not change individual tag hide states).
        - **Fixed Size** mode '1' (akin to original behavior).
        - **Glyph Scale** mode '2' scale is directly proportional to the node view size.
        - **Distance Scale** mode '3' scales, but closer is proportionally smaller.
    - Camera tag view settings are unique to each camera.
    - Camera settings do NOT affect the tag settings.
