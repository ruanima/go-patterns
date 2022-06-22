## Strategy

The Strategy pattern refers to behavioral patterns at the object level.

The Strategy pattern defines a set of similar algorithms, encapsulates them in a separate class, and makes them replaceable. The Strategy pattern allows you to replace algorithms without the participation of clients that use these algorithms.

Required for implementation:

1. The Context class, which is the context for the execution of a particular strategy;
2. The abstract class Strategy, which defines the interface of various strategies;
3. The ConcreteStrategyA class implements one of the strategies, which are algorithms aimed at achieving a specific goal;
4. The ConcreteStrategyB class implements one of the strategies, which are algorithms aimed at achieving a specific goal.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
