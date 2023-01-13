---
title: Slider
summary: A BlurLua class
---


A slider input

## Properties
| **Color** PressedColor |
| --------------------- |
| The color of the slider while its being pressed     |

| **number** MinValue |
| --------------------- |
| Minimum value that can be slidered to     |

| **Color** Color |
| --------------------- |
| Default color of the slider     |

| **Color** BackgroundHighlightedColor |
| --------------------- |
| Highlighted color of the background     |

| **number** Value |
| --------------------- |
| Current value selected by the slider     |

| **Color** BackgroundColor |
| --------------------- |
| Default background color of the slider     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Color** HighlightedColor |
| --------------------- |
| The color of the slider while it's hovered     |

| **number** MaxValue |
| --------------------- |
| Maximum value that can be slidered to     |

## Events
| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onValueChanged( **number** newValue ) |
| -------------------------- |
| Called when the value is changed |



