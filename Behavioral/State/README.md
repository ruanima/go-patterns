## State

The State pattern refers to behavioral patterns at the object level.

The State pattern allows an object to change its behavior based on its internal state and is an object-oriented implementation of a state machine. The object's behavior changes so much that it looks like the object's class has changed.

The pattern must be applied:

- when the behavior of an object depends on its state
- the behavior of the object must change during the execution of the program
- there are a lot of states and it is quite difficult to use conditional statements scattered throughout the code for this

Required for implementation:

1. The Context class is an object-oriented representation of a state machine;
2. The abstract class State, which defines the interface of various states;
3. The ConcreteStateA class implements one of the behaviors associated with a specific state;
4. The ConcreteStateB class implements one of the behaviors associated with a specific state.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also, Go uses composition instead of inheritance.

## -~- THE END -~-
