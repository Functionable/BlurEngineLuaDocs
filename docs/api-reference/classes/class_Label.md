---
title: Label
summary: A BlurLua class
---


A way of displaying text in GUIs

## Properties
| **Alignment** AlignmentX |
| --------------------- |
| Alignment of the text in the X axis     |

| **Alignment** AlignmentY |
| --------------------- |
| Alignment of the text in the Y axis     |

| **string** Text |
| --------------------- |
| The text displayed in the label     |

| **Color** Color |
| --------------------- |
| Determines the color of the text displayed     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

## Functions
| Label:setFont( **Font** font )  |
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



