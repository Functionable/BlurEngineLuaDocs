# Events

*If you're looking for the event library, go [here](libraries/event.md).*

BlurEngine has a rudimentary event system. This page should cover most, if not all events.

Lua Events can be called by any part of the code, and supply any kind of function. You can call these, but you really should be calling custom ones instead.

[TOC]

- - -

## GUI events

Events invoked by players' actions with GUI.

### checkedChanged

*Parameters: **none***

Executed when the checkbox was checked or unchecked.

### onPressed

*Parameters: **none***

Executed when the clickable GUI element was pressed.

### onSubmit

*Parameters: **none***

Executed when the TextBox's input was submitted.

## Input events

I don't think anything has to be said about these here, other than it'd be pretty difficult making a game without these.

### mouseMove

*Parameters: **int** X, **int** Y*

These are the absolute position of the mouse on the screen, not the delta position.

This event is called every time the mouse is moved on the screen.

### mouseClick

*Parameters: **BUTTON** key, **BUTTON_ACTION** action, **int** mods*

Key is the BUTTON enum which you can read about here (TODO: LINK)

Action is used to tell if the button was pressed, released, or held.

The mods parameter indicates whether keys like SHIFT or CTRL were also being pressed.

This event is called every time a button on the mouse is pressed.

### mouseScroll

*Parameters: **int** xscroll, **int** yscroll*

xscroll is used for devices that can scroll to the left/right

yscroll is what you most likely want to use. (Note: not always 1 or -1, you might want to clamp it if you're going to use this as a multiplier)

This event is called every time a scroll wheel is scrolled.

### passiveInput

*Parameters: **KEY** key, **BUTTON_ACTION** action*

Action is used to tell if the button was released, or pressed.

Key is the KEY enum which you can read about [here](enums.md).

This event is obviously called every time a button is pressed.

## Physics events

These events allow for Lua scripts to slightly hook into BlurEngine's physics engine.

### playerCollision

*Parameters: **Tile** tile, **Vector** direction*

This event is called every time the player object collides with a tile, the direction from which the player collides with the tile.

### playerCollision

*Parameters: **Vector** playerPos, **Vector** direction*

Called when the player collides with a tile, *playerPos* being the player's position at the time of collision and *direction* being the direction from the player to the other tile.

### onTileCollision

*Parameters:  **Tile** tile, **Vector** direction*

Called when a selected tile collides with another, *tile* is the tile being collided with, *direction* is the direction to it.

### doPhysics

*Parameters: **none**.*

If you're planning to do anything physics related every frame, I strongly recommend using this event rather than render, due to it being run in a different rendering phase, which might make whatever you're doing appear less wobbly.

## Screen events

These events are called to update GUIs or whatever else might depend on screen size/the render event.

### render

*Parameters: **none**.*

This event is called every frame.

### screenResize

*Parameters: **int** screenWidth, **int** screenHeight*

This event is called every time the window/screen is resized.