# BLF library

The BLF library is responsible for saving and loading using BLF, which is BlurEngine's own file format which can be used to store various data structures to aid the storage of level data.

## blf.findSaves

*Gets a table of all blf file names in the saves folder.*

| Returned  | Type   | Description                    | Example              |
| --------- | ------ | ------------------------------ | -------------------- |
| filePaths | table  | Table of .blf file paths found | {"saves/level1.blf"} |

## blf.load

*Reads a blf file at `saves/fileName` and returns all objects as a table.*

| Parameter | Type   | Description               | Example        | Required |
| --------- | ------ | ------------------------- | -------------- | -------- |
| fileName  | string | Name of the level loaded  | "level.blf"    | yes      |

| Returned | Type   | Description                   | Example          |
| -------- | ------ | ----------------------------- | ---------------- |
| objects  | table  | Table of objects in the level | A table of tiles |

## blf.save

!!! info
    This function will attempt to save it in a `saves/` folder.

!!! bug
    Writing a BLF file will fail if the saves directory is not present.

*Writes the *objects* table into a blf file named *fileName*.*

| Parameter | Type   | Description               | Example        | Required |
| --------- | ------ | ------------------------- | -------------- | -------- |
| fileName  | string | Name of the file saved to | "level.blf"    | yes      |
| objects   | table  | Table of objects saved    | Table of tiles | yes      |

## blf.version

| Returned | Type   | Description               | Example |
| -------- | ------ | ------------------------- | ------- |
| version  | string | The BLF Version available | "1.0.0" |