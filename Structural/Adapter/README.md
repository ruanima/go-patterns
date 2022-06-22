## Adapter

The Adapter pattern is a class-level structural pattern.

Often in a new project, developers want to reuse existing code. For example, existing classes may have the desired functionality but have incompatible interfaces. In such cases, the Adapter pattern should be used.

The meaning of this pattern is that if you have a class and its interface is not compatible with the code of your system, then in order to resolve this conflict, we do not change the code of this class, but write an adapter for it. In other words, Adapter adapts existing code to the required interface (is an adapter).

Required for implementation:

1. Target interface, describing the target interface (the interface with which our system would like to work);
2. The Adaptee class, which our system must adapt to itself;
3. The Adapter class, an adapter that implements the target interface.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
