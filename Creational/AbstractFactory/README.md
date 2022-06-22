## Abstract Factory

The Abstract Factory pattern is one of the object-level generative patterns.

The Abstract Factory pattern provides a common interface for creating a family of related objects. This allows you to separate the functionality of the system from the internal implementation of each class, and access to these classes becomes possible through abstract interfaces.

In general, an abstract factory looks like this. For each of the object families, a specific factory (the successor of the abstract one) is created, through which the products of this family are created.

Example: There are two soda factories, Coca-Cola and Pepsi. These factories produce a family of products (objects) - bottle, cap, label, liquid. Each of these factories produces products that interact with each other and cannot live separately from each other. The Coca-Cola Factory cannot supply empty bottles to customers.

To implement a simple creation of a family of objects, there must be an interface on which the factory works, and the factory must also release products with a specific interface. For example, the bottles of both companies have the same interface - they have a neck through which they are filled with liquid, we can also find out the volume of the bottles. Further, the bottles may differ in shape, volume or material, this does not concern us, we only need to know where to pour the liquid, as well as how much of this liquid is needed.

Required for implementation:

1. The abstract factory class AbstractFactory, which describes the general interface of the factory from which each specific factory will inherit;
2. The class of the abstract product AbstractProduct, which describes the general interface of the product, from which each specific product will be inherited;
3. The class of a specific factory Factory;
4. Product specific product class ProductA.
5. The specific product class ProductB.

Summarize.

An abstract factory is a base class that describes the interface of concrete factories that create products. Concrete factory classes derived from it must implement this interface.

Also, an abstract factory must describe the abstract products that it produces, so that specific factories produce products with the right interfaces.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
