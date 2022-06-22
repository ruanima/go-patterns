## Prototype

The Prototype pattern refers to object-level generative patterns.

The Prototype pattern allows you to create new objects by copying (cloning) the previously created object-original-product (prototype).

The pattern describes the process of creating clone objects based on the existing prototype object, in other words, the Prototype pattern describes how the cloning process is organized.

Required for implementation:

1. Base Prototype class declaring the cloning interface. All classes that inherit from it must implement this cloning mechanism;
2. Product class ConcretePrototypeA, which should implement this prototype;
3. Product class ConcretePrototypeB, which should implement this prototype.

Typically, the clone operation occurs through the clone() method, which is described in the base class and must be implemented by each product.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
