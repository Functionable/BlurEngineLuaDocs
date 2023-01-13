---
title: BLF Library
summary: BLF Library
---


A library for I/O using blur's own format: BLF, which allows for object definition and a few optimizations of how data is stored.n
!!! note 
	Functions in this library only operate within the `./saves/` directory.


| **table** findSaves(  )  |
| ------------------- |
| Returns a list of all BLF files that blur can find/access (in it's directory) |



| **table** generate( **table** object )  |
| ------------------- |
| Generates a blf definition table from the object given |



| **string** getVersion(  )  |
| ------------------- |
| Returns the current version of the BLF library in your blur build e.g: `1.1.0` |



| **table** load( **string** path )  |
| ------------------- |
| Returns a table of objects created through BLF. (loads from root dir) |



| save( **string** path, **any** valueTable )  |
| ------------------- |
| Saves a table of objects via BLF (note: in order to get saved, the objects have to have proper definitions, for more please view tutorials) |



