# Tile

Tiles are the most important part of your game. BlurEngine handles collisions and physics for you.

<img src="C:\Users\maxba\Desktop\Blur\BlurEngineLuaDocs\docs\images\tiles.png" align="left">

## Tile Class

The Tile class is used for creating tile objects.

### Functions

`.new()`

*Parameters: **Vector** position, **Texture** texture*

*Returns: **Tile** tile*

Creates a new tile.

**Deprecated** `tile.removeTile()`

*Parameters: **Tile** tile*

Removes the tile.





## Tile Object

The object created with the `tile.new` method

### Properties

#### Main

**Vector** Position

**Vector** Size

#### Physics

**bool** CollisionsEnabled

Decides whether the tile should collide with other tiles.

**bool** Static

If true, this tile cannot be moved by physics.

**Vector** Velocity

The speed and direction at which the tile should move. (see [Velocity](https://en.wikipedia.org/wiki/Velocity))

**Vector** Acceleration

The rate at which this tile gains or loses Velocity depending on if the value is negative. (also see [Acceleration](https://en.wikipedia.org/wiki/Acceleration))

**Vector** VelocityCeiling

The maximum velocity the tile can achieve.

**Vector** VelocityFloor

The minimum velocity the tile can achieve.

#### Visual

**Texture** Texture

**TEXTUREMODE** TextureMode

### Functions

`:duplicate()`

*Parameters: __none__*

Creates a copy of this tile.

`:remove()`

*Parameters: __none__*

Removes the tile (for older blur versions `tile.removeTile()` is used instead)



# Example

This example demonstrates how to make a basic tile then cause it to jump.

```lua
-- Register a texture to be used for the tile
crateTexture = texture.load("crate.png") 

-- Place a tile at 0,0 with the crate.png texture
crate = tile.new(Vector(0,0), crateTexture)

-- Set some physics properties to allow the jump
crate.VelocityFloor = Vector(0, -3) -- The crate will be brought to a full stop on the X axis, and will fall on the Y axis
crate.VelocityCeiling = Vector(1, 2) -- The max velocity (AKA the one at the start of the jump)
crate.Acceleration = Vector(-0.5, -4.4) -- Causes the tile to slow down and fall

function crate:Jump()
	crate.Velocity = Vector(1, 2) -- Jump to the right and up
end

crate:Jump()
```

## Practice:

When you run this script, the crate will jump up in the air and then fall down, however there is no floor to stop it.

Try making a floor using the `tile.Size` and `tile.TextureMode` properties.