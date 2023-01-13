---
title: GUI Library
summary: GUI Library
---


Contains all the functions required for your GUI-creation needs

| **GUI** new( **string** type )  |
| ------------------- |
| Instantiates a class deriving from GUI corresponding to the string |



| **GUIObject** newObject( **string** type )  |
| ------------------- |
| Instantiates a class deriving from GUIObject corresponding to the string (exception: Texture will instantiate GUITexture) |



| register( **GUI** gui )  |
| ------------------- |
| Adds a GUI to the base container (effectively, makes it visible on the screen) |



| unregister( **GUI** gui )  |
| ------------------- |
| Removes a GUI from the base container (effectively removes it from the screen) |



