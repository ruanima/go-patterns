## Factory method (FactoryMethod)

The Factory Method pattern refers to class-level generative patterns and focuses only on relationships between classes.

The Factory Method pattern is useful when a system must remain easily extensible by adding objects of new types. This pattern is the basis for all generative patterns and can be easily transformed to suit the needs of the system. Therefore, if the developer does not have clear requirements for the product or the way to organize interaction between products is not clear, then for a start you can use the Factory Method pattern until all the requirements are fully formed.

The Factory Method pattern is used to create objects with a specific interface whose implementations are provided by descendants. In other words, there is a base abstract factory class that says that each of its descendant factories must implement such and such a method in order to create their products.

The implementation of a factory method can be different, in most cases it depends on the implementation language. It can be polymorphism or a parameterized method.

Example: We receive files of three extensions .txt, .png, .doc. Depending on the file extension, we must save it in one of the /file/txt/, /file/png/ and /file/doc/ directories. So, we will have a file factory with a parameterized factory method that takes the path to the file that we need to save in one of the directories. This factory method returns us an object, using which we can manipulate our file (save, see the type and directory to save). Note that we do not specify in any way which instance of the product object we need to get, this is done by the factory method by determining the file extension and, based on it, choosing the appropriate product class. Thus, if our system expands and the available file extensions become, for example, 25, then we just need to change the factory method and implement the product classes.

Required for implementation:

1. The base abstract class Creator, which describes the interface that a specific factory must implement to produce products. This base class describes the factory method.
2. The base class Product, which describes the product interface that the factory returns. All products returned by the factory must adhere to the same interface.
3. The class of a specific factory for the production of ConcreteCreator products. This class must implement the factory method;
4. Real product class ConcreteProductA;
5. Real product class ConcreteProductB;
6. Real product class ConcreteProductC.

Factory Method differs from Abstract Factory in that Abstract Factory produces a family of objects, these objects are different, have different interfaces, but interact with each other. While the Factory Method produces products that adhere to the same interface and these products are not related to each other, do not interact.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
