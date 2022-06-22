## Template Method

The Template Method pattern refers to behavioral patterns at the class level.

The Template Method pattern forms the structure of the algorithm and allows derived classes to implement, override or redefine certain steps of the algorithm without changing the structure of the algorithm as a whole.

The designer decides which steps of the algorithm are fixed and which are changeable. The abstract base class implements the standard immutable steps of an algorithm and may provide a default implementation for mutable steps. Modifiable steps can be provided by the bean's client in concrete derived classes.

Required for implementation:

1. An abstract class AbstractClass that implements the Template Method, which describes the order of actions;
2. ConcreteClass class that implements changeable actions.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

Because in Go there is no concept of "Abstract Class" and the polymorphism familiar to us on inheritance, you should use the injection of a common type for the ConcreteClass with the implementation of the Template Method.

## -~- THE END -~-
