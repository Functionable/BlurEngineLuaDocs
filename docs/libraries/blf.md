# BLF library

[TOC]

## blf.findSaves

*Returns: __table__ existingSaves*

Gets a table of all blf file names in the saves folder.

## blf.load

*Parameters: __string__ fileName*
*Returns: __table__ objects*

Reads a blf file at *saves / fileName* and returns all objects as a table.

## blf.save

*Parameters: __string__ fileName, __table__ objects*

Writes the *objects* table into a blf file named *fileName*.

## blf.version

*Returns: __string__ blfVersion*

Returns the version of BLF somehow (Ask zmateusz).