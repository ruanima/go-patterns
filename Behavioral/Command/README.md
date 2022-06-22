## Command

The Command pattern refers to behavioral patterns at the object level.

The Command pattern allows you to represent a query as an object. It follows that a command is an object. Such requests, for example, can be queued, canceled or resumed.

In this pattern, we operate with the following concepts:
Command - request in the form of an object to be executed;
Receiver - the request receiver object that will process our command;
Invoker - the request initiator object.

The Command pattern separates the object that initiates the operation from the object that knows how to perform it. The only thing the initiator needs to know is how to send the command.

Required for implementation:

1. Base abstract class Command describing command interface;
2. ConcreteCommand class that implements the command;
3. The Invoker class, which implements the initiator, writes the command and provokes its execution;
4. The Receiver class, which implements the receiver and has a set of actions that the team can request;

Invoker can stack commands and initiate their execution on some event. By contacting the Invoker, you can cancel the command until it is executed.

ConcreteCommand contains requests to the Receiver that it must perform. In turn, the Receiver contains only a set of actions (Actions) that are performed when they are accessed from the ConcreteCommand.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
