---
title: Graph
summary: A BlurLua class
---


A nice way of displaying data

## Properties
| **string** Title |
| --------------------- |
| Title of the graph     |

| **integer** BottomValue |
| --------------------- |
| Minimum value (y = 0)     |

| **Color** Color |
| --------------------- |
| Color of the bars     |

| **Vector** Size |
| --------------------- |
| The on-screen size of the object     |

| **integer** TopValue |
| --------------------- |
| Maximum value (y = size.Y - padding)     |

| **bool** Visible |
| --------------------- |
| Determines whether the given object is drawn or not. Invisible objects cannot be interacted with.     |

| **integer** DisplayedCount |
| --------------------- |
| Max displayed data points at once     |

| **Vector** Position |
| --------------------- |
| The on-screen position of the object     |

## Functions
| Graph:resetData(  )  |
| ------------------- |
| Resets the graph's internal data array |



| Graph:addMarker( **integer** marker )  |
| ------------------- |
| Adds a marker at a specific value |



| Graph:addData( **integer** data )  |
| ------------------- |
| Adds a data point to the graph |



| Graph:resetMarker(  )  |
| ------------------- |
| Resets the graph's internal marker array |



## Events
| onEntered(  ) |
| -------------------------- |
| Called when the mouse starts hovering the object |



| onMouseMove( **Vector** mouseMove ) |
| -------------------------- |
| Called when the mouse moves |



| onLeave(  ) |
| -------------------------- |
| Called when the mouse stops hovering the object |



| onReleased(  ) |
| -------------------------- |
| This is called when the mouse stops clicking the object |



| onPressed(  ) |
| -------------------------- |
| This is called when the mouse clicks the object |



