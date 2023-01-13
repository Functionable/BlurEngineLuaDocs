---
title: WindowGUI
summary: A BlurLua class
---


The most complex GUI yet - the WindowGUI, comes with it's own `WindowDragger` and `ResizeDragger`

## Properties
| **string** Title |
| --------------------- |
| The window's displayed title     |

| **Vector** MinSize |
| --------------------- |
| The theoretical minimum size of the GUI, only used with objects that may resize the GUI     |

| **Color** Color |
| --------------------- |
| The Color of the GUI     |

| **Alignment** Alignment |
| --------------------- |
| Screen Alignment (determines which corner Position corresponds to)     |

| **number** Opacity |
| --------------------- |
| Degree to which the GUI's background is transparent     |

| **bool** BlurBackground |
| --------------------- |
| Determines whether the background of the GUI should be blurred     |

| **Vector** Size |
| --------------------- |
| The size of the GUI on the screen (measured with pixels)     |

| **Color** DraggerColor |
| --------------------- |
| The color of the window dragger     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Vector** MaxSize |
| --------------------- |
| Only used with `ResizeDragger`, the 'theoretical maximum size' of your GUI     |

| **Vector** Position |
| --------------------- |
| Relative location of your GUI on the screen (measured in pixels)     |

## Functions
| WindowGUI:addObject( **GUIObject** object )  |
| ------------------- |
| Adds an `object` to the GUI |



| WindowGUI:setExitVisible( **bool** newState )  |
| ------------------- |
| Changes the visibility of the window's exit button |



| WindowGUI:removeObject( **GUIObject** object )  |
| ------------------- |
| Removes an `object` from the GUI |



## Events
| onClosed(  ) |
| -------------------------- |
| Called when the window is closed (GUI is unregistered) |



| onResize( **Vector** oldSize, **Vector** newSize ) |
| -------------------------- |
| Called when the GUI is resized. |



| onUnfocused(  ) |
| -------------------------- |
| Called when the GUI is no longer focused. |



| onFocused(  ) |
| -------------------------- |
| Called when the GUI is focused. |



