---
title: TileRenderer
summary: A BlurLua class
---


The tile renderer class, it's job is pretty easy, though it may require a lot of parameters

## Functions
| TileRenderer:renderTileRotated( **Texture** texture, **Color** color, **Vector** position, **Vector** size, **Vector** textureSize, **bool** isTextureTiled, **number** angleRad, **number** opacity )  |
| ------------------- |
| Renders a tile just like `renderTile` but allows you to specify the rotation about it's center |



| TileRenderer:renderTile( **Texture** texture, **Color** color, **Vector** position, **Vector** size, **Vector** textureSize, **bool** isTextureTiled, **number** opacity )  |
| ------------------- |
| Renders a tile, without the tile object. Please ensure opacity is a number that is 0-1 |



