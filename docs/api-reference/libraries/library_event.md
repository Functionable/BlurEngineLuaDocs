---
title: event Library
summary: event Library
---


Event library, in charge of everything to do with events.

| call( **string** eventID, **varargs** eventArgs )  |
| ------------------- |
| Calls all functions registered to the event with provided `eventArgs` |



| link( **string** eventID, **string** functionID, **function** eventFunction )  |
| ------------------- |
| Adds a function, with it's own identifier to an event's function pool, so that it can be called when the event is called. |



| register( **string** eventID )  |
| ------------------- |
| Registers an event name to blur's event manager. |



