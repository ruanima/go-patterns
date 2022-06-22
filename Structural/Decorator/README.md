## Decorator

The Decorator pattern is an object-level structural pattern.

The Decorator pattern is used to extend the functionality of objects by dynamically adding new features to an object. When implementing the pattern, the relation of composition is used.

The essence of the work of the decorator is to wrap the finished object with new functionality, while the entire original interface of the object remains available, by passing the decorator all requests to the wrapped object.

Required for implementation:

1. The base abstract class Component which provides an interface for the decorator class and the component;
2. The ConcreteDecorator class, which implements the Component interface and reloads all methods of the component, adding functionality to them if necessary;
3. The ConcreteComponent class that implements the Component interface and will be wrapped with a decorator.

With such a structure, it doesn’t matter to us whether the component is a decorator or a specific implementation, since they have the same interface, and we can make chains of decorators. Thus dynamically change the state and behavior of the object.

I heard the Kalson example and I really liked it. We have Carlson, we put on him overalls, thereby changing his state, then we put a propeller on his pants, thereby changing his behavior. The propeller, depending on the situation, can be removed by changing the behavior to the opposite, or you can wear another suit with different properties.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
