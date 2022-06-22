## Proxy

The Proxy pattern is one of the object-level structural patterns.

The Proxy pattern provides an object to control access to another object.

Another name for the pattern is "Surrogate". In this sense, it is an object or product that replaces some other object or product with which the surrogate has only some properties in common, but does not have all the qualities of the original object or product.

The Proxy pattern puts forward a number of important requirements, namely that the original object and its surrogate must interact with each other, and it must also be possible to replace the surrogate with the original object at the place of its use, respectively, the interaction interfaces of the original object and its surrogate must match.

It will be easier for you to understand the pattern if you have watched the movie "The Surrogates".

Required for implementation:

1. Subject interface, which is a common interface for a real object and its surrogate;
2. RealSubject class that implements a real object;
3. The Proxy class that implements the surrogate object. Stores a reference to a real object, which allows the proxy to access the real object directly;

For example, the Proxy pattern can be used if we need to manage resource-intensive objects, but we do not want to create instances of such objects until they are actually used.

You might think that this is the same as Adapter or Decorator. But...

The proxy exposes the same interface to its object.
Adapter provides a different interface.
Decorator provides an extended interface.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
