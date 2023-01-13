---
title: Button
summary: A BlurLua class
---


A button, you press it, you get an event

## Properties
| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

| **Color** PressedColor |
| --------------------- |
| The color of the button while its being pressed     |

| **string** Text |
| --------------------- |
| Text displayed on the button     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Color** HighlightedColor |
| --------------------- |
| The color of the button while it's hovered     |

| **Color** Color |
| --------------------- |
| Default color of the button     |

## Functions
| Button:setFont( **Font** font )  |
| ------------------- |
| Sets the object's font |



## Events
| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



