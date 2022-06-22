## Observer

The Observer pattern refers to object-level behavioral patterns.

The Observer pattern defines a one-to-many dependency between objects so that when the state of one object changes, all dependent objects are notified and updated automatically.

The main participants of the pattern are Publishers (Subject) and Subscribers (Observer).

There are two ways to receive notifications from a publisher:

1. Pull method: After receiving notification from the publisher, the subscriber must go to the publisher and retrieve (pull) the data themselves.
2. Push method: The publisher does not notify the subscriber of data updates, but delivers (push) the data to the subscriber on its own.

Required for implementation:

1. An abstract class Subject that defines the interface of the Publisher;
2. ConcreteSubject class, implements the Subject interface;
3. An abstract Observer class that defines the general functionality of Subscribers;
4. The ConcreteObserver class, implements the Subscriber;

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
