## Composite

The Composite pattern is one of the object-level structural patterns.

The Composite pattern groups similar objects into tree structures.

To build the tree, arrays representing the branches of the tree will be used.

Required for implementation:

1. The base abstract class Component which provides an interface for both branches and leaves of the tree;
2. The Composite class, which implements the Component interface and is a branch of the tree;
3. The Leaf class, which implements the Component interface and is a leaf of the tree.

Note that a tree leaf is a leaf node class and cannot have children (a leaf cannot grow into a branch or another leaf).

The branches of the tree define the behavior of the objects included in the structure of the tree, which have children, and also store the components of the tree themselves. In other words, branches can contain other branches and leaves.

The main purpose of the pattern is to provide a single interface to both the composite (branch) and final (leaf) object, so that the client does not think about what object he is working with.

[!] In the description of the pattern, general concepts are used, such as Class, Object, Abstract class. Applied to the Go language, these are a User Type, a Value of that Type, and an Interface. Also in the Go language, aggregation and inlining are used instead of conventional inheritance.

## -~- THE END -~-
