---
title: Load & Save
layout: home
nav_order: 4
parent: Managing Datascape Projects
---

### Load Dataset or Asset

- **1, 2 or 3** - key loads a preset dataset specified in:
    - `/User/_Global_/csv/np_preset.csv`
- **L** - key for **Open File Dialog** to load a specific dataset or asset:
    - **Alt+L** - load dataset (as children) onto the currently active glyph.
    - To load entire dataset, choose the `[dataset]_npe.bat` file.
    - Single assets can be loaded by selecting the specific file:
        - Native CSV tables, eg. `[dataset]_np_node.csv`
        - 3D Models will also attempt to load their specified texture.
        - Texture formats (PNG, TIFF...) support transparency.
- Assets (images, 3D models, ...) are loaded at startup from:
    - `/User/_Global_/[subfolders]`

### Save Methods


- **Shift+[#]** (1, 2 or 3) - save current dataset scene and set it as a preset (#).
    - Legacy presets are moved and transformed to the current dataset schema.
- **K** - for **Save As File Dialog** (prompts with default dataset name).
    - eg. `/User/Prototypes/2024-01-31/proto-20240131T090341/'
        - Can change the folder location and dataset name as preferred.
    - Screenshot of current camera view is put in the base folder (with [dataset].bat).
    - Subfolders are created for each asset type:
        - eg. `/User/proto/2024-01-31/[dataset]/csv/[dataset]_node.csv`
        - *Note, shared assets in `/User/_Global_/[subfolders]` are not copied.
- **Ctrl+K** - saves a copy with ver number (or as proto if no active dataset).
- **Alt+K** or **Alt+Shift+(1, 2 or 3)** - Save only the currently selected glyphs.
    - Note that branches will be saved as root objects with their local coordinates.
- **[Save Selected]** - Toolbar button will save selected items to a node table.
    - **L-click** to save ONLY selected nodes (with relative local coordinates).
    - **R-click** to save selected nodes with all sub-branches.
- **F4** - Save Screenshot to the currently active (last used) dataset base folder.
    - **Shift+F4** - Screenshot saved with alpha transparency using RGBA TIFF.

### Launching Built-In Visualizations


- **4** - Reserved for custom viz (eg. Edge-AI demo).
- **5** - FileViz directory tree, choose root folder (**Alt+5** uses 'usr/fileviz').
- **6** - GitViz issues from a github repo (specified in npglobals.csv).
- **7** - Color palettes with a node for each index color.
- **Alt+7** - Test Scene (generates 250K+ varied nodes).

### Quit Program
- **Alt+F4** - Quit without saving.

---