## Facade

The Facade pattern is an object-level structural pattern.

The Facade pattern provides a high-level unified interface in the form of a set of method names to a set of related classes or objects of some subsystem, which makes it easier to use.

Breaking a complex system into subsystems simplifies the development process, and also helps to minimize the dependencies of one subsystem on another. However, it becomes quite difficult to use such subsystems. One way to solve this problem is the Facade pattern. Our task is to make a simple, unified interface through which one could interact with subsystems.

An example is the car interface. Modern cars have a unified interface for the driver, which hides a complex subsystem. Thanks to the use of sophisticated electronics that do most of the work for the driver, he can easily drive a car without thinking about how everything works there.

Required for implementation:

1. Facade class providing unified access for subsystem classes;
2. Subsystem class SubSystemA;
3. Subsystem class SubSystemB;
4. Subsystem class SubSystemC.

Note that the façade is not the only access point to the subsystem, nor does it restrict what "advanced" users may want to work with the subsystem directly.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
