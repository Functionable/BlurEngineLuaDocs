---
title: File Library
summary: File Library
---


Allows you to write/read content from the user's drive, if you do not wish to use BLF. 

!!! note 
	Functions in this library only work within blur's core directory. Access outside of that is disallowed for security reasons.


| **bool** exists( **string** path )  |
| ------------------- |
| Determines whether a given path to a file exists on the filesystem |



| **array** listDir( **string** path )  |
| ------------------- |
| Recursively iterates over a given directory and returns the list of files contained within |



| **string** load( **string** path )  |
| ------------------- |
| Loads entire file as string (path relative to blur root) |



| save( **string** path, **string** contents )  |
| ------------------- |
| Saves string as file (path relative to blur root) |



