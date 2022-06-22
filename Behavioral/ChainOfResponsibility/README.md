## Chain Of Responsibility

The Chain Of Responsibility pattern refers to behavioral patterns at the object level.

The Chain Of Responsibility pattern allows you to avoid binding the request sender object to the request recipient object, while giving several objects a chance to process this request. The recipients are connected in a chain, and the request is passed along the chain until it is processed by some object.

In essence, this is a chain of handlers that receive a request in turn, and then decide whether to process it or not. If the request is not processed, then it is passed down the chain. If it is processed, then the pattern itself decides to pass it on or not. If the request is not processed by any handler, then it is simply lost.

Required for implementation:

1. The base abstract class Handler, which describes the interface of handlers in chains;
2. Class ConcreteHandlerA, which implements a specific handler A;
3. Class ConcreteHandlerB, which implements a specific handler B;
4. The ConcreteHandlerC class, which implements a specific C handler;

Note that instead of storing links to all candidate recipients of a request, each sender keeps a single link to the beginning of the chain, and each receiver has a single link to its successor, the next element in the chain.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
