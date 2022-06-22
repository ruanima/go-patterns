## Singleton

The Singleton pattern is one of the object-level generative patterns.
The pattern controls the creation of a single instance of a certain class and provides access to it.
In other words, Singleton guarantees that the class will have only one instance and provides an access point to it, through a factory method.

Required for implementation:

1. The GetInstance function, which creates an instance of the Singleton class only once. If an instance has already been created before then simply returns that instance.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
