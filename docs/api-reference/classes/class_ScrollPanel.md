---
title: ScrollPanel
summary: A BlurLua class
---


A scrollable panel, if you ever needed MORE space

## Properties
| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

## Functions
| ScrollPanel:addObject( **GUIObject** object )  |
| ------------------- |
| Adds an `object` to the ScrollPanel |



| ScrollPanel:removeObject( **GUIObject** object )  |
| ------------------- |
| Removes an `object` from the ScrollPanel |



## Events
| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



