---
title: CheckBox
summary: A BlurLua class
---


!!! warning 

	Prior to Alpha 1.5.0, this class was called `Checkbox`, if scripting for an older version or simply upgrading your scripts to a newer version do ensure you catch this difference!


## Properties
| **Color** CheckHighlightedColor |
| --------------------- |
| Highlighted color of the check     |

| **Color** CheckColor |
| --------------------- |
| Default color of the check     |

| **Color** Color |
| --------------------- |
| Default color of the checkbox     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **bool** Checked |
| --------------------- |
| Determines whether the checkbox is checked     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Color** HighlightedColor |
| --------------------- |
| Highlighted color of the checkbox     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

## Events
| onCheckedChanged( **bool** newState ) |
| -------------------------- |
| Called when the checked state is changed |



| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



