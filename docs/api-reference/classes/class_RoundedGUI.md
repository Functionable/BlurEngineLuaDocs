---
title: RoundedGUI
summary: A BlurLua class
---


A GUI, but rounded!

## Properties
| **Vector** MaxSize |
| --------------------- |
| Only used with `ResizeDragger`, the 'theoretical maximum size' of your GUI     |

| **bool** RoundTopCorners |
| --------------------- |
| Determines whether the top corners should be rounded     |

| **Vector** MinSize |
| --------------------- |
| The theoretical minimum size of the GUI, only used with objects that may resize the GUI     |

| **number** Radius |
| --------------------- |
| Size of the rounded corners     |

| **number** Opacity |
| --------------------- |
| Degree to which the GUI's background is transparent     |

| **Color** Color |
| --------------------- |
| The Color of the GUI     |

| **bool** BlurBackground |
| --------------------- |
| Determines whether the background of the GUI should be blurred     |

| **Vector** Size |
| --------------------- |
| The size of the GUI on the screen (measured with pixels)     |

| **bool** RoundBottomCorners |
| --------------------- |
| Determines whether the bottom corners should be rounded     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Alignment** Alignment |
| --------------------- |
| Screen Alignment (determines which corner Position corresponds to)     |

| **Vector** Position |
| --------------------- |
| Relative location of your GUI on the screen (measured in pixels)     |

## Functions
| RoundedGUI:addObject( **GUIObject** object )  |
| ------------------- |
| Adds an `object` to the GUI |



| RoundedGUI:removeObject( **GUIObject** object )  |
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



