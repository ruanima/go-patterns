## Bridge

The Bridge pattern is an object-level structural pattern.

The Bridge pattern allows you to separate an object into an abstraction and an implementation so that they can change independently of each other.

If several implementations are possible for one abstraction, then inheritance is usually used. However, this approach is not always convenient, since inheritance tightly binds the implementation to the abstraction, which makes it difficult to independently modify and complicate their reuse.

The pattern should be applied when we have an abstraction and several of its implementations. Of course, it makes no sense to separate abstraction from implementation if there can be only one implementation.

I did not find any adequate description of the "Bridge" pattern. Everything that I have come across either does not correspond to reality and the examples are sucked from the finger or very blurry. From what I understand and can explain on my fingers - the Bridge is a tricky aggregation. The class that implements the product implements the interface of the aggregated class, which is slipped at the stage of creating an instance of the product class.

As I understand it... we have 3 cars and 3 different engines. Every engine fits every car, i.e. it implements its interface. If we do this by inheritance, we will get 9 different classes. It turns out that each car has 3 modifications. This is inconvenient, so we will slip the engine at the stage of creating the car. Also, each engine can run on different fuels, diesel or gasoline, so as not to produce 6 different implementations, when creating an engine, we will slip the type of fuel into it.

To implement the pattern in this example, it is necessary to add a field in the base class of cars to store a pointer to the type of implementation, the value of which the class will receive in its constructor, and call the methods of the nested object as necessary.

Required for implementation:

1. Base abstract class (in our case, describing a car);
2. A class that implements the base class. It has a property in which we will slip a pointer to the engine used (the machine can work with any of the engines presented);
3. Engine abstraction;
4. Implementation of the engine.

In general, a property that stores a pointer to the object used is a bridge. We can slip different objects into it, the main thing is that they have the same interface.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, instead of conventional inheritance, aggregation and inlining are used.

## -~- THE END -~-
