---
title: Global Functions
summary: All Globals
---

This page documents all functions present directly in _G.
It does not document any libraries which are available in another section.


| **Vector** Vector( **number** x, **number** y, **number** z (optional) )  |
| ------------------- |
| Creates a new Vector object. The z component is optional. |

| assert( **bool** v, **string** message )  |
| ------------------- |
| Causes an error if `v` is `false`. If `true`, it returns all of it's arguments`. If an error is caused, the optional argument `message` is the error message. |

| collectgarbage( **string** opt, **any** arg )  |
| ------------------- |
| Lua has many ways it can do garbage collection. This function can invoke some of those ways. The optional argument `opt` corresponds to which method will be used (as specified [here](https://www.lua.org/manual/5.4/manual.html#pdf-collectgarbage)). The optional argument `arg` is passed to the chosen garbage collection method. |

| delay( **number** delay, **function** function )  |
| ------------------- |
| Calls a function after a delay. Does not block the execution of Lua code. |

| error( **any** message, **any** level )  |
| ------------------- |
| Terminates the last protected function called and returns `message` as the error object. Function `error` never returns.  |

| **table** findmetatable( **string** name )  |
| ------------------- |
| Retrieves a C metatable with a given name |

| **integer** getBuildNumber(  )  |
| ------------------- |
| Returns the build number of the binary running this code. Can be used to 'detect' features. |

| **number** getDeltaTime(  )  |
| ------------------- |
| Returns the delta (time difference) between this and last frame in seconds. |

| **integer** getHeight(  )  |
| ------------------- |
| Returns the window's height (in pixels) |

| **string** getVersionString(  )  |
| ------------------- |
| Returns the current build's version string, for example: ```Alpha 1.2.0-pre (master)``` |

| **integer** getWidth(  )  |
| ------------------- |
| Returns the width of the game window (in pixels) |

| **metatable** getmetatable( **any** object )  |
| ------------------- |
| Will return `nil`. Will return the metatable of the object if __metatable is not present, if __metatable is present, returns the value returned by that function |

| include( **string** scriptPath )  |
| ------------------- |
| Loads a Lua script. Note that `scriptPath` has to be an absolute path from `./scripts/` |

| **variable** ipairs( **table** t )  |
| ------------------- |
| Returns three values: an iterator function, `t` and 0. |

| **table** listblurmetatables(  )  |
| ------------------- |
| Returns a dictionary of all blur metatables (keys: names, values: metatables) |

| **function** load( **string** chunk )  |
| ------------------- |
| Allows for a binary chunk to be loaded into a function. |

| log( **string** name, **string** content, **LogSeverity** severity )  |
| ------------------- |
| Same as ```print```, offers more granular control when outputting to the console. |

| **variable** next( **table** table, **number** index )  |
| ------------------- |
| Returns the next index of the table and the value at that index. If `index` is nil, next returns an initial index and the value at that index. If `index` is the last index, or the table is empty, nil is returned |

| **variable** pairs( **table** t )  |
| ------------------- |
| If t has the `__pairs` metamethod, it will call it with t as the argument and return first three results from the call. If it does not contain the metamethod, it will return the next function, `t` and `nil`. |

| **variable** pcall( **function** f, **variable** args )  |
| ------------------- |
| Calls the `f` in protected mode. In the case of an error, a differing status code is returned. If called without errors, the return values after the status code are `f`'s return values. |

| print( **variable** any )  |
| ------------------- |
| Will log any variable provided in the console. Internally will use similar behaviour ```tostring``` to convert passed variables to a string. |

| rawequal( **any** object1, **any** object2 )  |
| ------------------- |
| Checks if two objects specified are equal to each other without calling the `__eq` metamethod. |

| **any** rawget( **table** table, **any** index )  |
| ------------------- |
| Gets the value of `table[index]` without calling the `__index` metamethod. |

| **number** rawlen( **any** v )  |
| ------------------- |
| Returns the length of `v` (which is expected to a table or string) without calling the `__len` metamethod. |

| rawset( **table** table, **any** index, **any** value )  |
| ------------------- |
| Sets the value of table[index] without using the `__newindex` metamethod. |

| **module** require( **string** path )  |
| ------------------- |
| Loads a Lua module at a given path. May not work very well currently. It is planned to be fixed in the next patch. |

| **variable** select( **number** index )  |
| ------------------- |
| This function can accept any number of arguments after index. It will return all arguments whose argument index is larger than `index` |

| setBackgroundColor( **Color** backgroundColor )  |
| ------------------- |
| Sets the 2D view's background color. |

| setIcon( **string** iconPath )  |
| ------------------- |
| Sets the game window's icon to the image at the path given. |

| setTitle( **string** title )  |
| ------------------- |
| Sets the game window's title to the string provided. |

| **table** setmetatable( **table** table, **table** metatable )  |
| ------------------- |
| Sets the metatable for the given table. If the metatable specified is `nil`, the metatable is removed from the givent able. If the original metatable has a `__metatable` metafunction, it will cause an error. |

| **Vector** toScreenVector( **Vector** worldVector )  |
| ------------------- |
| This function will return the screen coordinates `worldVector`'s world space representation. |

| **Vector** toWorldVector( **Vector** screenVector )  |
| ------------------- |
| Converts a vector in screen space to a vector in world space |

| **number** tonumber( **object** any )  |
| ------------------- |
| A lua standard library function that attempts to convert it's argument to a number. If the passed argument cannot be converted ```nil``` is returned. |

| **string** tostring( **object** any )  |
| ------------------- |
| A lua standard library function that attempts to convert any type into a string for metatables it will attempt to call the metatable's ```__tostring``` metamethod. |

| **string** type( **object** any )  |
| ------------------- |
| Returns the type of an object, passing a Tile would return ```Tile```.</br>Or ```type(12)``` would return ```number``` |

| warn( **variable** values )  |
| ------------------- |
| Shows a warning where the message is all the arguments passed to this function concatenated. |

| **variable** xpcall( **function** f, **function** msgh, **variable** args )  |
| ------------------- |
| Calls `f` just like `pcall`, however an error will call the message handles `msgh`. |

