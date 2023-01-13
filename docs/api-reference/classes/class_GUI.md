---
title: GUI
summary: A BlurLua class
---


Base GUI class

## Properties
| **Vector** MaxSize |
| --------------------- |
| Only used with `ResizeDragger`, the 'theoretical maximum size' of your GUI     |

| **Vector** MinSize |
| --------------------- |
| The theoretical minimum size of the GUI, only used with objects that may resize the GUI     |

| **Color** Color |
| --------------------- |
| The Color of the GUI     |

| **bool** BlurBackground |
| --------------------- |
| Determines whether the background of the GUI should be blurred     |

| **Vector** Size |
| --------------------- |
| The size of the GUI on the screen (measured with pixels)     |

| **Vector** Position |
| --------------------- |
| Relative location of your GUI on the screen (measured in pixels)     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **number** Opacity |
| --------------------- |
| Degree to which the GUI's background is transparent     |

| **Alignment** Alignment |
| --------------------- |
| Screen Alignment (determines which corner Position corresponds to)     |

## Functions
| GUI:addObject( **GUIObject** object )  |
| ------------------- |
| Adds an `object` to the GUI |



| GUI:removeObject( **GUIObject** object )  |
| ------------------- |
| Removes an `object` from the GUI |



## Events
| onResize( **Vector** oldSize, **Vector** newSize ) |
| -------------------------- |
| Called when the GUI is resized. |



| onUnfocused(  ) |
| -------------------------- |
| Called when the GUI is no longer focused. |



| onFocused(  ) |
| -------------------------- |
| Called when the GUI is focused. |



