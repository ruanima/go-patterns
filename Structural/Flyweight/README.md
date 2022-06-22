## Flyweight

The Flyweight pattern is an object-level structural pattern.

The Flyweight pattern is used to efficiently support a large number of small objects, it allows you to reuse small objects in different contexts.

Required for implementation:

1. The FlyweightFactory class, which is a modified factory pattern for creating flyweights;
2. The base abstract class Flyweight, to describe the general interface of flyweights;
3. The ConcreteFlyweight class that implements a flyweight that will replace identical small objects.

The bottom line is that we can request flyers from the factory on request, in turn, it will give those objects that have already been created, or create new ones. This means that we will use the already created objects, and not create even more if the objects we need already exist. It is also worth noting that opportunists have an internal and external state. The factory finds flyers by its internal state, and the external state is passed to its methods.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
