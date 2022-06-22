## Visitor

The Visitor pattern is an object-level behavioral pattern.

The Visitor pattern allows you to bypass a set of elements (objects) with heterogeneous interfaces, and also allows you to add a new method to the object class without changing the class of this object itself.

Required for implementation:

1. Abstract class Visitor, describing the interface of the visitor;
2. The ConcreteVisitor class, which implements a specific visitor. Implements methods for traversing a particular element;
3. The ObjectStructure class, which implements the structure (collection) in which the elements to be traversed are stored;
4. Abstract class Element, which implements the interface of structure elements;
5. The ElementA class, which implements the element of the structure;
6. The ElementB class that implements the structure element.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
