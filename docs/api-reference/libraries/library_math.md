---
title: math Library
summary: math Library
---


Contains maths functions and constants for your convenience

| **number** abs( **number** x )  |
| ------------------- |
| Returns the absolute value of a given number. |



| **number** acos( **number** x )  |
| ------------------- |
| Returns the arc cosine of a given value (x is assumed to be in radians) |



| **number** asin( **number** x )  |
| ------------------- |
| Returns the arcsine of `x` in radians |



| **number** atan( **number** y, **number** x )  |
| ------------------- |
| Equivalent to atan2 in most languages. Returns the arctangent of y/x. This operation is done in radians |



| **number** ceil( **number** x )  |
| ------------------- |
| Rounds up to the nearest integer |



| **number** clamp( **number** value, **number** min, **number** max )  |
| ------------------- |
| Clamps `value` between `min` and `max` |



| **number** cos( **number** x )  |
| ------------------- |
| Returns the cosine of `x` (which is assumed to be in radians) |



| **number** deg( **number** angRad )  |
| ------------------- |
| Converts a given value (assumed to be in radians) to degrees |



| **number** exp( **number** x )  |
| ------------------- |
| Returns the value of e^x |



| **number** floor( **number** x )  |
| ------------------- |
| Rounds down a given number to the nearest integer. |



| **number** fmod( **number** x, **number** y )  |
| ------------------- |
| Returns the remainder of the division of x by y |



| huge <span style="float: right;">Constant: inf</span> |
| ------------------- |
| A float with the largest possible numeric value |

| **number** log( **number** x, **number** base )  |
| ------------------- |
| Returns the logarithm of `x` in a given base. The argument `base` is optional (and defaults to e if not specified) |



| **number** max( **variable** numbers )  |
| ------------------- |
| Returns the highest number between all the arguments. A variable amount of arguments may be passed to this function |



| maxinteger <span style="float: right;">Constant: 9223372036854775807</span> |
| ------------------- |
| An integer with the largest possible value |

| **number** min( **variable** numbers )  |
| ------------------- |
| Returns the lowest number between all the arguments. A variable amount of arguments may be passed to this function |



| mininteger <span style="float: right;">Constant: -9223372036854775808</span> |
| ------------------- |
| An integer with the lowest possible value |

| **numbers** modf( **number** x )  |
| ------------------- |
| Returns the integral part of `x` and the fractional part of `x`. The second result is always a float |



| pi <span style="float: right;">Constant: 3.1415926535898</span> |
| ------------------- |
| Contains the value of PI |

| **number** rad( **number** angDeg )  |
| ------------------- |
| This function converts the given angle (assumed to be in degrees) to radians |



| **number** random( **number** m, **number** n )  |
| ------------------- |
| If no arguments are specified, it returns a number between 0 and 1. If `m` and `n` are specified, it will return a number between m and n. |



| randomseed( **number** x, **number** y )  |
| ------------------- |
| Initializes Lua's pseudo-random number generator with the given value. If `y` is specified, it is combined with `x` into one number that is then used as the seed for the PRNG. |



| **integer** round( **number** value )  |
| ------------------- |
| Rounds a value to the nearest integer |



| **number** sin( **number** x )  |
| ------------------- |
| Calculates the sine of `x`, `x` is assumed to be in radians |



| **number** sqrt( **number** x )  |
| ------------------- |
| Calculates the square root of `x` |



| **number** tan( **number** x )  |
| ------------------- |
| Returns the tangent of `x` (assumed to be in radians) |



| **integer** tointeger( **number** x )  |
| ------------------- |
| Turns a number into an integer. If value that is not a number is specified, it returns fail. |



| **string** type( **number** x )  |
| ------------------- |
| Returns `"integer"` if a given number is an integer, `"float"` if the value is a float or `nil` otherwise |



| **bool** ult( **number** m, **number** n )  |
| ------------------- |
| Returns `true` if `m < n` when m and n are compared as unsigned integers |



