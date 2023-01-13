---
title: table Library
summary: table Library
---


This default Lua library contains additional functions that help with table manipulation

| **string** concat( **table** table, **string** sep, **number** i, **number** j )  |
| ------------------- |
| Concatenates all elements in a given table into a string. All arguments after table are optional. `sep` is the separator between each entry, while `i` and `j` are the start and end bounds between which all elements will be concatenated into a string. |



| insert( **table** list, **number** pos, **any** value )  |
| ------------------- |
| This function inserts a value into a table at a specified `pos`. The `pos` is an optional argument and if not specified, the function assumes that `pos` is at the end of the table. |



| **table** move( **table** table1, **number** startIndex, **number** endIndex, **number** otherStart, **table** table2 )  |
| ------------------- |
| Returns table2. It moves elements from `table1` (between `startIndex` and `endIndex`) to `table2` (from `otherStart` onwards), `table2` is an optional argument, and if not specified, `table2` is assumed to be `table1`. |



| **table** pack( **variable** any )  |
| ------------------- |
| This function accepts any number of arguments. It will then create and return a new table containing all of these arguments. |



| remove( **table** table, **number** index )  |
| ------------------- |
| Removes an element from a table at a given index. The `index` is optional, and if not specified it defaults to the end of the table. This function modifies the table passed and therefore does not modify anything. |



| sort( **table** table, **function** sort )  |
| ------------------- |
| This function sorts a table. It modifies the table specified and therefore does not return anything. It also accepts an optional argument `sort` which should be a function taking two arguments that is able to sort the table. More information on how this function works can be found [here](https://www.lua.org/manual/5.4/manual.html#pdf-table.sort) |



| **variable** unpack( **table** list, **number** start, **number** end )  |
| ------------------- |
| Returns the elements in the list. The arguments `start` and `end` are optional. |



