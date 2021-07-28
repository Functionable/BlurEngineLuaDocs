# Events

*If you're looking for the event library, go [here](libraries/event.md).*

BlurEngine has a rudimentary event system. This page should cover most, if not all events.

Lua Events can be called by any part of the code, and supply any kind of function. You can call these, but you really should be calling custom ones instead.

[TOC]

- - -

## GUI methods

Events invoked by players' actions with GUI.

### :checkedChanged

*Parameters: __none__*

Executed when the checkbox was checked or unchecked.

### :onPressed

*Parameters: __none__*

Executed when the clickable GUI element was pressed.

### :onSubmit

*Parameters: __none__*

Executed when the TextBox's input was submitted.

## Input events

I don't think anything has to be said about these here, other than it'd be pretty difficult making a game without these.

### mouseMove

*Parameters: __int__ X, __int__ Y*

These are the absolute position of the mouse on the screen, not the delta position.
This event is called every time the mouse is moved on the screen.

### mouseClick

*Parameters: __BUTTON__ key, __BUTTON_ACTION__ action, __int__ mods*

This event is called every time a button on the mouse is pressed.
Key is the BUTTON [enum](enums.md). 
Action is used to tell if the button was pressed, released, or held.
The mods parameter indicates whether keys like SHIFT or CTRL were also being pressed.

### mouseScroll

*Parameters: __int__ xscroll, __int__ yscroll*

This event is called every time a scroll wheel is scrolled.
*xscroll* is used for devices that can scroll to the left/right
*yscroll* is what you most likely want to use. (Note: not always 1 or -1, you might want to clamp it if you're going to use this as a multiplier)

### passiveInput

*Parameters: __KEY__ key, __BUTTON_ACTION__ action*

Action is used to tell if the button was released, or pressed.
Key is the KEY [enum](enums.md).
This event is obviously called every time a button is pressed.

## Physics events

These events allow for Lua scripts to slightly hook into BlurEngine's physics engine.

### doPhysics

*Parameters: __none__*

If you're planning to do anything physics related every frame, I strongly recommend using this event rather than render, due to it being run in a different rendering phase, which might make whatever you're doing appear less wobbly.

## Physics methods

These are members of tiles.

### :onTileCollision

*Parameters:  __Tile__ tile, __Vector__ direction*

Called when this tile collides with another, *tile* is the tile being collided with, *direction* is the direction to it.

### [DEPRECATED] :playerCollision

*Parameters: __Vector__ playerPos, __Vector__ direction*

Called when the player collides with a tile, *playerPos* being the player's position at the time of collision and *direction* being the direction from the player to the other tile.

## Screen events

These events are called to update GUIs or whatever else might depend on screen size/the render event.

### render

*Parameters: __none__*

This event is called every frame.

### screenResize

*Parameters: __int__ screenWidth, __int__ screenHeight*

This event is called every time the window/screen is resized.