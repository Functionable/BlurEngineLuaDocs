# Global functions

There are many global functions with different applications.

Most of them affect either the player tile or the game window, as well as providing some kind of useful functionality.

[TOC]

- - -

## Tile functions

Currently there are two of them, but they're some of the most important.

### tile.new

*Parameters: **Vector** position, **Texture** texture*
*Returns: **Tile** addedTile*

Adds a new tile at *position*, with the *texture* texture and returns it.

### tile.remove

*Parameters: **Tile** targetTile*

Removes *targetTile*.
Currently still removeTile.

## Debugging functions

These functions can be used to display useful debug messages in the game view or command prompt.

### print

*Parameters: **any** value*

Displays *value* in the command prompt which runs alongside the game view.

### displayMessage

*Parameters: **string** message*

Displays *message* in the engine's logging UI.
Deprecated.

### displayMessageWithTime

*Parameters: **string** message, **number** length*

Displays *message* in the engine's logging UI, fading away after *length* seconds.
Deprecated.

## Utility functions

Used mostly to get constants, for delays and conversion.

### getBuildNumber

*Returns: **int** buildNumber*

Returns the current build number with each new release being 1 greater than the last.

### getVersionString

*Returns: **string** version*

Returns the current version as a string in the form of 1.2.3.

### delay

*Parameters: **number** delay, **function** delayedFunc*

Executes *delayedFunc* in *delay* seconds.

### getDeltaTime

*Returns: **number** deltaTime*

Returns delta time of current frame, should be used in physics/render events.
Multiply by 10 to convert it to seconds.

### toWorldVector

*Parameters: **Vector** screenCoordinates*
*Returns: **Vector** convertedCoordinates*

Converts a screen coordinate, usually from the mouse, into a coordinate in the world.

## Game view & window functions

Modify the game view or application window.

### setBackgroundColor

*Parameters: **number** r, **number** g, **number** b*

Sets the game view's background color to a new RGB color created from *r*, *g* and *b*.

### setTitle

*Parameters: **string** newTitle*

Sets the window's title text to *newTitle*.

### setIcon

*Parameters: **Texture** newIcon*

Sets the window's icon to *newIcon*.

## Camera functions

### camera.setPosition

*Parameters: **Vector** newPosition*

Moves the game camera to *newPosition*.

### camera.track

*Parameters: **Tile** target*

Makes the camera follow *target*.

## [DEPRECATED] Player functions

Player functions affect only the player tile, which, for some reason, is treated separately from other tiles.

### setEngineMovementState

*Parameters: **bool** movementState*

Enables or disables the engine's pre-existing top-down movement.

### getPlayerMovementDirection

*Returns: **Vector** playerMovementDirection*

### setPlayerCollisions

*Parameters: **bool** collide*

Enables or disables the player tile's collider.

### getPlayerPos

*Returns: **Vector** playerPos*

### setPlayerPos

*Parameters: **Vector** newPlayerPos*

### getPlayerTexture

*Returns: **Texture** playerTexture*

### setPlayerTexture

*Parameters: **Texture** newPlayerTexture*

### getPlayerVelocity

*Returns: **Vector** playerVelocity*

### setPlayerVelocity

*Parameters: **Vector** newPlayerVelocity*

### getPlayerVelocityFloor

*Returns: **Vector** playerVelocityFloor*

### setPlayerVelocityFloor

*Parameters: **Vector** newPlayerVelocityFloor*

### getPlayerVelocityCeiling

*Returns: **Vector** playerVelocityCeiling*

### setPlayerVelocityCeiling

*Parameters: **Vector** newPlayerVelocityCeiling*

### getPlayerDrag

*Returns: **Vector** playerDrag*

This is actually 'acceleration'.

### setPlayerDrag

*Parameters: **Vector** newPlayerDrag*

This is actually 'acceleration'.