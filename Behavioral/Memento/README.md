## Keeper (Memento)

The Memento pattern refers to object-level behavioral patterns.

The Memento pattern retrieves and stores outside of an object its internal state so that the object can later be restored to the same state. If the client later needs to "roll back" the state of the original object, it passes Memento back to the original object to restore it.

The pattern operates on three objects:

1. The owner of the state (Originator);
2. Keeper (Memento) - Stores the state of the host object of the Originator class;
3. Caretaker - Responsible for the safety of the object-custodian of the Memento class.

Required for implementation:

1. The Originator class, which has some kind of changing state, and it can also create and receive keepers (Memento) of its state;
2. The Memento class, implements storage for the Originator state;
3. The Caretaker class, receives and stores the custodian object (Memento) until the owner needs it.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
