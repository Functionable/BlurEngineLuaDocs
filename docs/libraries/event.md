# Event Library

*If you were looking for global events, click [here](../events.md).*

## event.call

*Parameters: __string__ eventName, __any__ arguments*

Calls *eventName* with *arguments*.

## event.link

*Parameters: __string__ eventName, __string__ uniqueIdentifier, __function__ function*

Links *function* to the *eventName* given in the event system.

*uniqueIdentifier* can be any string.

## event.register

*Parameters: __string__ eventName*

Registers the *eventName* in the event manager.