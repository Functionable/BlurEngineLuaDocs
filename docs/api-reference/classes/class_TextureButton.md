---
title: TextureButton
summary: A BlurLua class
---


A button and a GUITexture in one

## Properties
| **Color** TextureColor |
| --------------------- |
| The color used to tint the TextureButton's `Texture`     |

| **string** Text |
| --------------------- |
| Text displayed on the button     |

| **Texture** Texture |
| --------------------- |
| The texture displayed     |

| **Color** Color |
| --------------------- |
| Default color of the button     |

| **Vector** TextureSize |
| --------------------- |
| Size of the texture (in pixels) (the texture is always centered)     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **Color** PressedColor |
| --------------------- |
| The color of the button while its being pressed     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Color** HighlightedColor |
| --------------------- |
| The color of the button while it's hovered     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

## Functions
| TextureButton:setFont( **Font** font )  |
| ------------------- |
| Sets the object's font |



## Events
| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



