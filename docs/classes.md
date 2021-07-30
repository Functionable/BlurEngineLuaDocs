# Classes

## Tile

### Fields

#### Main

**Vector** Position

**Vector** Size

#### Physics

**bool** CollisionsEnabled

Does this tile collide with other objects?

**bool** Static

If true, this tile cannot be moved by physics.

**Vector** Acceleration

The rate at which this tile gains speed.

**Vector** Velocity

**Vector** VelocityCeiling

**Vector** VelocityFloor

#### Visual

**Texture** Texture

**TEXTUREMODE** TextureMode

### Functions

**duplicate**

*Parameters: __none__*

Creates a copy of this tile.

## GUI

There are different types of GUI that have their own classes.

### Shared properties

**Vector** Position

**Vector** Size 

**ALIGN** Alignment

### Shared methods

**addObject**

*Parameters: __GUIObject__* object

Adds a GUIObject to the parent GUI class object.

### GUI

Normal GUI class, includes a square frame with no additional features.

#### WindowGUI

Includes a square frame with additional features such as dragging, resizing, a title and close button .

#### RoundedGUI

Includes a rounded frame with no additional features.

#### GUIObject

All usable GUI elements have different features and thus their own classes.

## GUIObject

There are many different GUIObjects that differ in function, thus they have their own classes.

### Shared properties

**Vector** Position

**Vector** Size 

**ALIGN** Alignment

### Button

#### Functions

**:setFont**

*Parameters: __string__ fontName, __number__ fontSize*

Sets the font type and size used to display this Button's text.

**:onPressed**

Parameters: **none**

This function is fired when the button is clicked. You have to define it like so:

```lua
-- Let button be a GUIObject of class Button
function button:onPressed()
	print("I just got pressed!")
end
```



### Checkbox

#### Fields

**bool** Checked

### Graph

#### Fields

**int** DisplayedCount

The number of points displayed on the graph.

**number** BottomValue

**number** TopValue

**string** Title

#### Functions

**addData**

*Parameters: __int__ dataPoint*

**addMarker**

*Parameters: __int__ marker*

**resetData**

*Parameters: __none__ *

**resetMarker**

*Parameters: __none__ *

### Label

#### Fields

**string** Text

#### Functions

**:setFont**

*Parameters: __string__ fontName, __int__ fontSize*

Sets the font type and size used to display this Label's text.

### ProgressBar

#### Fields

**int** Percentage

### Slider

#### Fields

**int** Value

**int** MinValue

**int** MaxValue

### Textbox

#### Fields

**string** Text

#### Functions

**:setFont**

*Parameters: __string__ fontName, __int__ fontSize*

Sets the font type and size used to display this Textbox's text.

**submit**

*Parameters: __none__*

Submit the current input text.

### Texture

#### Fields

**Texture** Texture



