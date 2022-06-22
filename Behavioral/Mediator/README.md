## Mediator

The Mediator pattern is an object-level behavioral pattern.

The Mediator pattern provides a mediator object that hides the way that many other peer objects interact. Mediator makes the system loosely coupled by eliminating the need for objects to refer to each other, which allows you to change the interaction between them independently.

For example, we have an intermediary between a bakery factory, a farmer, and a distribution store. The intermediary saves the farmer from interacting with the factory that uses his raw materials, and the factory from interacting with the store, which receives products for sale.

Required for implementation:

1. Interface Mediator - an intermediary describing the organization of the process for the exchange of information between objects of the Colleague type;
2. The ConcreteMediator class that implements the Mediator interface;
3. The base abstract class Colleague - a colleague that describes the organization of the process of interaction of colleague objects with an object of Mediator type;
4. The ConcreteColleague class that implements the Colleague interface. Each peer object only knows about the mediator object. All peer objects exchange information only through an intermediary.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
