---
title: TileType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# TileType : [[ClassEnum]]

The kinds of tile that make up a [[TileMap]]. Each type sets a tile's appearance and its movement costs — including which characters can cross it and how expensive doing so is. New tile types are loaded from asset files.

## Enum values
| Id  | Name              | Texture path    | Movement costs         | Description |
| --- | ----------------- | --------------- | ---------------------- | ----------- |
| 10 | [[Grass]] | tile/grass1.png | Default: 0  | Open ground; free to walk across. |
| 11 | [[Out of bounds]] | tile/black.png |   | The area off the map; impassable to everyone. |
| 12 | [[Water]] | tile/water1.png | Flying: 0  | Only flying units can cross; blocks everyone else. |
| 13 | [[Dirt]] | tile/dirt1.png | Flying: 0, Default: 10  | Costly for those on foot; free for flyers. |
| 14 | [[Sand]] | tile/sand1.png | Default: 0  | Open ground; free to walk across. |
| 15 | [[Mud]] | tile/dirt2.png | Default: 0  | Open ground; free to walk across. |


