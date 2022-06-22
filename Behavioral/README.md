## Behavioral patterns

Behavioral patterns are divided into two types:

1. Class Level Patterns
2. Object level patterns.

Class level patterns describe interactions between classes and their subclasses. Such relationships are expressed through inheritance and implementation of classes. Here the base class defines the interface, and the subclasses define the implementation.

Object level patterns describe interactions between objects. Such relations are expressed by links - association, aggregation and composition. Here, structures are built by combining objects of some classes.

Association - a relationship when objects of two classes can refer to one another. For example, a class property contains an instance of another class.

Aggregation is a particular form of association. Aggregation is used when one object should be a container for other objects and the lifetime of these objects does not depend in any way on the lifetime of the container object. In general, if the container is destroyed, then the objects included in it will not be affected. For example, we created an object, and then passed it to the container object, in some way, you can transfer it to the method of the container object or assign it directly to the container property from the outside. This means that when deleting the container, we will not affect our created object in any way, which can interact with other containers.

Composition - Same as aggregation, but compound objects cannot exist separately from the container object, and if the container is destroyed, then all its contents will be destroyed too. For example, we created an object in a container object method and assigned it to a container object property. From the outside, no one knows about our created object, which means that when the container is deleted, the created object will be deleted in the same way, because there is no external reference to it.

Only the "Template Method" applies to class-level patterns.

Behavioral patterns describe the interaction of objects and classes with each other and try to achieve the least degree of interconnection of system components with each other, making the system more flexible.

* [Chain Of Responsibility](ChainOfResponsibility)
* [Command (Command)](Command)
* [Iterator (Iterator)](Iterator)
* [Mediator](Mediator)
* [Keeper (Memento)](Memento)
* [Observer (Observer)](Observer)
* [State (State)](State)
* [Strategy](Strategy)
* [Template Method](TemplateMethod)
* [Visitor](Visitor)

## -~- THE END -~-
