---
title: Socket
summary: A BlurLua class
---


A network socket that can act as a server or client

## Functions
| Socket:listen( **int** backlog )  |
| ------------------- |
| Begins listening for client connections, `backlog` being the length of the pending connections buffer |



| Socket:connect( **string** address, **number** port )  |
| ------------------- |
| Connects to a server at the specified `address` and `port` |



| **Socket** Socket:accept(  )  |
| ------------------- |
| Accepts a pending client connection in a listening server socket |



| Socket:close(  )  |
| ------------------- |
| Closes and cleans up after the socket |



| **string** Socket:read( **integer** length )  |
| ------------------- |
| Reads `length` bytes and puts them in a string and then returns the string |



| **bool** Socket:endReached(  )  |
| ------------------- |
| Returns `true` only if End Of Stream has been reached |



| **integer** Socket:bind( **string** address, **number** port )  |
| ------------------- |
| Binds a server socket to a local address (to which clients can connect to) |



| **number** Socket:available(  )  |
| ------------------- |
| Returns the number of bytes queued up to be read |



| Socket:write( **string** data, **integer** length )  |
| ------------------- |
| Writes data in string to the socket |



| **bool** Socket:isConnected(  )  |
| ------------------- |
| Returns a bool indicating whether the socket is connected to a server/client. |



