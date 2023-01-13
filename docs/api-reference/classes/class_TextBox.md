---
title: TextBox
summary: A BlurLua class
---


A way of inputting text

## Properties
| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **Color** TextColor |
| --------------------- |
| Specifies the color of the text in the textbox     |

| **string** Text |
| --------------------- |
| Text contained by the textbox     |

| **Color** Color |
| --------------------- |
| Default color of the textbox     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **Color** HighlightedColor |
| --------------------- |
| Highlighted color of the textbox     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

## Functions
| TextBox:setFont( **Font** font )  |
| ------------------- |
| Sets the object's font |



| TextBox:submit(  )  |
| ------------------- |
| Submits the text in the textbox, calls the submit event |



## Events
| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onSubmitted(  ) |
| -------------------------- |
| Called when `:submit()` is called by something |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onCommand( **string** command ) |
| -------------------------- |
| An input is interpreted as a command when it should perform something else other than end up in an input. For example: while this TextBox is capturing input, pressing `KEY_HOME` will result in this event being called with `HOME` as the argument. |



| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



