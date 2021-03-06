# Classes

[TOC]

## Tile

### Fields

#### Main

**Vector** Position
**Vector** Size

#### Physics

**bool** CollisionsEnabled
Does this tile collide with other objects?

**bool** Static
Does this tile get moved by physics?

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

*Parameters: **none***

Creates a copy of this tile.


## GUI

All usable GUI elements have different features and thus their own classes.

### Shared members
**Vector** Position
**Vector** Size 
**ALIGN** Alignment

### Button

#### Functions

**:setFont**

*Parameters: **string** fontName, **int** fontSize*

Sets the font type and size used to display this Button's text.

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

*Parameters: **int** dataPoint*

**addMarker**

*Parameters: **int** marker*

**resetData**

*Parameters: **none***

**resetMarker**

*Parameters: **none***

### Label

#### Fields

**string** Text

#### Functions

**:setFont**

*Parameters: **string** fontName, **int** fontSize*

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

*Parameters: **string** fontName, **int** fontSize*

Sets the font type and size used to display this Textbox's text.

**submit**

*Parameters: **none***

Submit the current input text.

### Texture

#### Fields

**Texture** Texture