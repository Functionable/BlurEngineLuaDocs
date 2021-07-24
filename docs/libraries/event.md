# event library

*If you were looking for global events, click [here](../events.md).*

[TOC]

## event.call

*Parameters: **string** eventName, **any** arguments*

Calls *eventName* with *arguments*.

## event.link

*Parameters: **string** eventName, **string** uniqueIdentifier, **function** function*

Links *function* to the *eventName* given in the event system.

## event.register

*Parameters: **string** eventName*

Registers the *eventName* in the event manager.