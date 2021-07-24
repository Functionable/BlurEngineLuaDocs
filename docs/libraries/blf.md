# BLF library

[TOC]

## blf.findSaves

*Returns: **table** existingSaves*

Gets a table of all blf file names in the saves folder.

## blf.load

*Parameters: **string** fileName*
*Returns: **table** objects*

Reads a blf file at *saves / fileName* and returns all objects as a table.

## blf.save

*Parameters: **string** fileName, **table** objects*

Writes the *objects* table into a blf file named *fileName*.

## blf.version

*Returns: **string** blfVersion*

Returns the version of BLF somehow (Ask zmateusz).