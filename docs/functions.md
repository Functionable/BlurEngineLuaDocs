# Global functions

There are many global functions with different applications.

Most of them affect either the player tile or the game window, as well as providing some kind of useful functionality.

[TOC]

- - -

## Tile functions

Currently there are two of them, but they're some of the most important.

### tile.new

*Parameters: __Vector__ position, __Texture__ texture*
*Returns: **Tile** addedTile*

Adds a new tile at *position*, with the *texture* texture and returns it.

### tile.remove

*Parameters: __Tile__ targetTile*

Removes *targetTile*.
Currently still removeTile.

## Debugging functions

These functions can be used to display useful debug messages in the game view or command prompt.

### print

*Parameters: __any__ value*

Displays *value* in the command prompt which runs alongside the game view.

### displayMessage

*Parameters: __string__ message*

Displays *message* in the engine's logging UI.
Deprecated.

### displayMessageWithTime

*Parameters: __string__ message, __number__ length*

Displays *message* in the engine's logging UI, fading away after *length* seconds.
Deprecated.

## Utility functions

Used mostly to get constants, for delays and conversion.

### getBuildNumber

*Returns: __int__ buildNumber*

Returns the current build number with each new release being 1 greater than the last.

### getVersionString

*Returns: __string__ version*

Returns the current version as a string in the form of 1.2.3.

### delay

*Parameters: __number__ delay, __function__ delayedFunc*

Executes *delayedFunc* in *delay* seconds.

### getDeltaTime

*Returns: __number__ deltaTime*

Returns delta time of current frame, should be used in physics/render events.
Multiply by 10 to convert it to seconds.

### toWorldVector

*Parameters: __Vector__ screenCoordinates*
*Returns: __Vector__ convertedCoordinates*

Converts a screen coordinate, usually from the mouse, into a coordinate in the world.

## Game view & window functions

Modify the game view or application window.

### setBackgroundColor

*Parameters: __number__ r, __number__ g, __number__ b*

Sets the game view's background color to a new RGB color created from *r*, *g* and *b*.

### setTitle

*Parameters: __string__ newTitle*

Sets the window's title text to *newTitle*.

### setIcon

*Parameters: __Texture__ newIcon*

Sets the window's icon to *newIcon*.

## Camera functions

### camera.setPosition

*Parameters: __Vector__ newPosition*

Moves the game camera to *newPosition*.

### camera.track

*Parameters: __Tile__ target*

Makes the camera follow *target*.

## [DEPRECATED] Player functions

Player functions affect only the player tile, which, for some reason, is treated separately from other tiles.

### setEngineMovementState

*Parameters: __bool__ movementState*

Enables or disables the engine's pre-existing top-down movement.

### getPlayerMovementDirection

*Returns: __Vector__ playerMovementDirection*

### setPlayerCollisions

*Parameters: __bool__ collide*

Enables or disables the player tile's collider.

### getPlayerPos

*Returns: __Vector__ playerPos*

### setPlayerPos

*Parameters: __Vector__ newPlayerPos*

### getPlayerTexture

*Returns: __Texture__ playerTexture*

### setPlayerTexture

*Parameters: __Texture__ newPlayerTexture*

### getPlayerVelocity

*Returns: __Vector__ playerVelocity*

### setPlayerVelocity

*Parameters: __Vector__ newPlayerVelocity*

### getPlayerVelocityFloor

*Returns: __Vector__ playerVelocityFloor*

### setPlayerVelocityFloor

*Parameters: __Vector__ newPlayerVelocityFloor*

### getPlayerVelocityCeiling

*Returns: __Vector__ playerVelocityCeiling*

### setPlayerVelocityCeiling

*Parameters: __Vector__ newPlayerVelocityCeiling*

### getPlayerDrag

*Returns: __Vector__ playerDrag*

This is actually 'acceleration'.

### setPlayerDrag

*Parameters: __Vector__ newPlayerDrag*

This is actually 'acceleration'.