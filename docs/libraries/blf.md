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

!!! info
    This function will attempt to save it in a `saves/` folder.

!!! bug
    Writing a BLF file will fail if the saves directory is not present.

Writes the *objects* table into a blf file named *fileName*.

| Prameter | Type   | Description               | Example        | Required |
| -------- | ------ | ------------------------- | -------------- | -------- |
| fileName | string | Name of the file saved to | "level.blf"    | yes      |
| objects  | table  | Table of objects saved    | Table of tiles | yes      |

## blf.version

| Returned | Type   | Description               | Example |
| -------- | ------ | ------------------------- | ------- |
| version  | string | The BLF Version available | "1.0.0" |