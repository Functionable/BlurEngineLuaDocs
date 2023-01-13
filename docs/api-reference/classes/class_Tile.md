---
title: Tile
summary: A BlurLua class
---


A tile

## Properties
| **number** Density |
| --------------------- |
| Affects how much velocity is transferred to it in a collision     |

| **Vector** Static |
| --------------------- |
| Determines if it's velocity/acceleration can be changed or altered by the environment     |

| **Vector** Velocity |
| --------------------- |
| The rate of change of position     |

| **TextureMode** TextureMode |
| --------------------- |
| Display mode of the texture     |

| **Texture** Texture |
| --------------------- |
| The rendered texture     |

| **Vector** VelocityCeiling |
| --------------------- |
| The highest velocity can go     |

| **Vector** Acceleration |
| --------------------- |
| The rate of change of velocity     |

| **Vector** TextureSize |
| --------------------- |
| Size of the texture, works when tiled     |

| **bool** CollisionsEnabled |
| --------------------- |
| Whether or not the collision system acts on the tiles (onCollide will still be called if false)     |

| **Vector** Size |
| --------------------- |
| The world size of the Tile     |

| **Vector** VelocityFloor |
| --------------------- |
| The lowest velocity can go     |

| **Color** Color |
| --------------------- |
| The color that the Tile can be tinted with     |

| **number** Friction |
| --------------------- |
| When moving against another tile, a force diminishing the current velocity will be accounted for, scaled by this property     |

| **Vector** Position |
| --------------------- |
| Where in the world the vector is located     |

## Events
| onCollision( **Tile** tile, **Vector** collisionNormal ) |
| -------------------------- |
| Called when a tile collides with another tile |



