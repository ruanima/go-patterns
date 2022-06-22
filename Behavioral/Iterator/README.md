## Iterator

The Iterator pattern refers to behavioral patterns at the object level.

The Iterator pattern provides a mechanism for traversing collections of objects without exposing their internal representation.

Often this pattern is used instead of an array of objects to not only provide access to the elements, but also to endow with some logic.

Iterator is a generic interface that allows you to implement arbitrary iteration logic.

Required for implementation:

1. Iterator interface describing a set of methods for accessing a collection;
2. The ConcreteIterator class that implements the Iterator interface. Tracks the position of the current element while iterating through the collection (Aggregate).;
3. The Aggregate interface describing a set of methods for collecting objects;
4. The ConcreteAggregate class, which implements the Aggregate interface and stores the elements of the collection.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
