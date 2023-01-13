---
title: string Library
summary: string Library
---


This is a standard Lua library that aids with string manipulation

| **numbers** byte( **string** s, **number** startIndex, **number** endIndex )  |
| ------------------- |
| Returns numeric codes of characters between given indices in a string. Both `startIndex` and `endIndex` are entirely optional arguments. |



| **string** char( **variable** values )  |
| ------------------- |
| Takes an arbitrary amount of number arguments. It returns a string with each character's code corresponding to the argument given |



| **string** dump( **function** function, **bool** strip )  |
| ------------------- |
| Returns a string containing the binary representation of a given function. If `strip` is specified and is set to true, the binary output may not have all debug information |



| **numbers** find( **string** s, **string** pattern, **number** i, **bool** plain )  |
| ------------------- |
| Both `i` and `plain` are optional arguments. This function searches string `s` for `pattern`, starting from `i` (assumed to be 1 if not specified). If `plain` is specified and `true` then no special pattern matching is done and this function simply searches for `pattern` in the string. The start and end of the first found occurence are returned. Pattern matching is done according to the section [here](https://www.lua.org/manual/5.4/manual.html#6.4.1). |



| **string** format( **string** fmt )  |
| ------------------- |
| Formats a string in the same fashion as C's `sprintf` would. Any number of variables after `fmt` may be passed. |



| **function** gmatch(  )  |
| ------------------- |
| Returns an interator function that returns the next capture from the pattern each time it is called. The `pattern` specification is [here](https://www.lua.org/manual/5.3/manual.html#6.4.1). |



| **string** gsub( **string** s, **string** pattern, **any** repl, **number** n )  |
| ------------------- |
| To understand how this function works, I recommend you read [this](https://www.lua.org/manual/5.3/manual.html#pdf-string.gsub). |



| **number** len( **string** s )  |
| ------------------- |
| Returns the length of a given string. |



| **string** lower( **string** string )  |
| ------------------- |
| Returns a copy of the string given with all possible letters set to lowercase. |



| match( **string** s, **string** pattern, **number** index )  |
| ------------------- |
| Searches the string for the first match of a given pattern. Starts from the optional `index`. Rules of `format` are [here](https://www.lua.org/manual/5.3/manual.html#6.4.1) |



| **string** pack( **string** fmt, **variable** values )  |
| ------------------- |
| Many variables may be specified after `fmt`. The function returns a binary string containing all the values but serialized. The format used for `fmt` can be found [here](https://www.lua.org/manual/5.4/manual.html#6.4.2) |



| **number** packsize( **string** format )  |
| ------------------- |
| Returns the size of a string that would result from a given `format` |



| **string** rep( **string** s, **integer** n, **string** sep )  |
| ------------------- |
| Returns a string that is the concatenation of `n` copies of string `s` separated by `sep` (which is optional, and if missing is assumed to be an empty string) |



| **string** reverse( **string** string )  |
| ------------------- |
| Returns a reversed copy of a given string |



| **string** sub( **string** string, **number** i, **number** j )  |
| ------------------- |
| Returns a substring between `i` and `j`. The argument `j` is optional |



| **number** unpack( **string** fmt, **string** s, **integer** pos )  |
| ------------------- |
| Returns values packed in string s, according to `string.pack`, and [format string](https://www.lua.org/manual/5.3/manual.html#6.4.2) `fmt`. The optional argument `pos` specifies where to start reading from (1 by default). |



| **string** upper( **string** string )  |
| ------------------- |
| Returns a copy of this string with all the letters turned uppercase. |



