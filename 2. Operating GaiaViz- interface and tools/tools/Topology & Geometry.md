---
title: Topology & Geometry
parent: Tools
layout: home
nav_order: "3"
---
Use topology and geometry parameter to organize the structure of the hyperglyph: geometry is the shape an object takes, and the topology is the structure that defining how the sub-objects distribute around it.


# Topology & Geometry

| Hotkeys   | Functions                                                |
| --------- | -------------------------------------------------------- |
| J         | Next '**topo**' type, **Shift+J** for previous topo.     |
| Alt+J     | will change which parent facet (on a cube...).           |
| **O**     | Object geometry, does not change the 'topo' type.        |
| **ALT+G** | Set current glyph node to be a grid (topo and geometry). |
|           |                                                          |


## In grid mode :

| Hotkeys | Functions                                                                          |
| ------- | ---------------------------------------------------------------------------------- |
| **Y**   | Increases the (Grid) **`segment_x y z`** count (**Shift+Y** - decreases the count) |
| Z       | (**`segment_z`**) is stacks of grids as 3D layers.                                 |
|         |                                                                                    |

- Hint: If X & Y segments = 1, the grid is an empty rectangle.
- Actions ONLY apply to the **active axes** (**X** key) component(s).
- **ALT+Y** - increase unit size spacing (**Shift+Alt+Y** to decrease).
    - **`np_node`** table stores (grid) spacing (`**np_node**` table: **`auxa_x y z`**).
    - Total grid dimensions are determined by the grid **spacing X segments = length** (per axis).
