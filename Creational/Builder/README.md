## Builder

The Builder pattern is one of the object-level generative patterns.

The Builder pattern defines the process of building a complex product in stages. After the last part of it is built, the product can be used.

The Abstract Factory pattern example provided an example of two factories, Coca-Cola and Percy. Let's take one factory, it produces a complex product consisting of 4 parts (cap, bottle, label, drink) that must be applied in the right order. You can’t first take a cap, a bottle, screw the cap on, and then try to pour a drink into it. To implement an object, a bottle of Coca-Cola that is delivered to a client, we need a Builder pattern.

It is important to understand that a complex object is not necessarily an object that operates on several other objects in the OOP sense. For example, we need to get a document consisting of a title, introduction, content and conclusion. Our document is a complex object. In order to have some kind of uniform order for compiling a document, we will use the Builder pattern.

Required for implementation:

1. The Director class, which will manage the builder and give him commands in the right order, and the builder will execute them;
2. The base abstract class Builder, which describes the interface of the builder, the commands that it must execute;
3. The ConcreteBuilder class, which implements the builder interface and interacts with the complex object;
4. The class of the complex object Product.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, instead of conventional inheritance, aggregation and inlining are used.

## -~- THE END -~-
