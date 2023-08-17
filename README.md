# CPP-Laboratory-Work

LAB 1:

Define a class "Set" that represents a dynamically allocated, expandable collection of integer data of type "int". The set is considered an unordered collection of data without duplicates (provide checks and constraints). Two sets are considered equal if every element belonging to one set also belongs to the other, regardless of their order in memory. The class should have methods for:

Adding an element to the set.
Removing an element from the set.
Checking if an object belongs to the set.
Printing all elements of the set.
Comparing two sets for equality.
Enable the initialization of an empty set using the default constructor. Properly handle memory reallocation when adding new elements or removing elements from the set.

========================================================

LAB 2:

Define a class "Rectangle" that represents a rectangle aligned with the axes in 2D space. Allow the rectangle to be positioned anywhere in space. Define the following operators:

• Operator +, so that adding two rectangles produces their minimal bounding rectangle, i.e., the rectangle of minimal area that contains both rectangles (allowing the edges of the new rectangle to touch the edges of the operand rectangle).

• Commutative operator * for scaling the rectangle with respect to the intersection point of its diagonals (center of the rectangle), so that scaling by X produces a rectangle whose area is X times larger than the area of the operand rectangle, while maintaining the same aspect ratio of sides.

• Bitwise AND operator (&), so that it returns the intersection of two rectangles (also a rectangle).

Suggestion: When implementing the + and & operators, consider using the maximum and minimum coordinate values of vertices along the x and y axes.

Define a class "Set" that represents an unlimited set of rectangles. The set is unordered and has no duplicates. Properly define operators for:

Adding an element to the set.
Removing an element from the set.
Printing all elements of the set.
Comparing two sets for equality.
When printing, a sequence of ordered triplets (center, side a, side b) should be displayed. Allow the use of operators in a constant context.

========================================================

LAB 3:

Define an interface with default behavior that enables the printing of objects to an output stream using the output operator, without the need to overload the operator for implementing classes. Define an interface that allows the comparison of objects using relational operators. Define an interface for representing 2D shapes that can be compared based on their perimeter and whose relevant data can be printed to an output stream. Define an interface for objects that can be positioned in 2D space, whose coordinates can be printed to an output stream, and that can be compared based on their distance from the origin. Enable working with rectangles and squares in 2D space aligned with the coordinate axes. Enable working with circles in 2D space. Enable working with arbitrary polygons (polygons with an arbitrary number of points) in 2D space. For all these shapes, it should be possible to calculate the perimeter, compare them based on the perimeter, and compare them based on the distance from the origin. Demonstrate different ways of comparing some of the shapes. The shapes should implement the appropriate interfaces.

Define a class that represents an unlimited unordered set of elements, where the elements can be of an arbitrary (from the perspective of the class user) polymorphic type from this task. Define a class that represents an unlimited "sorted" set of elements of an arbitrary polymorphic type from this task. As an implementation detail, this set always contains elements in sorted order and allows for fast search and output in sorted order. Define a class that represents an unlimited "comparable" set of elements of an arbitrary polymorphic type from this task, which can be compared using the "is subset" relation with relational operators. Define a class for representing a set that simultaneously has the characteristics of a sorted set and a comparable set. For all set types, ensure proper definition of methods and/or operators for:

-Adding an element to the set.
-Removing an element from the set.
-Printing all elements of the set.
-Comparing two sets for equality.
-Filtering elements of the set.
-Performing an action on all elements of the set.
-Transforming elements of the set such that the image of each element can be an arbitrary polymorphic type from this task (one method).

========================================================

LAB 4:

Define a generic class for an unlimited set of elements (without duplicates) of an arbitrary polymorphic type. The class template for the set includes methods for adding elements: add and tryAdd. It also includes methods for removing elements: remove and tryRemove. The add method should throw an exception if the object being attempted to add already exists in the set. The remove method should throw an exception if the object being attempted to remove does not exist in the set. The tryAdd and tryRemove methods do not throw exceptions but return a boolean value to signal success.

Define a class that represents a sorted set, so that it only supports elements with a defined ordering relation (compile-time constraint – requires operators <, >, <=, and >=).

In the main program function, demonstrate all functionalities.

(Note: I've provided a general translation based on the description you provided. The specific implementation details may vary based on the programming language you are using.)

========================================================

LAB 5:

Define a generic class Graph<T> for working with undirected graphs. Implement the following functionalities:

Adding and removing nodes
Adding and removing edges between nodes
Depth-First Search (DFS) traversal using iterators, allowing user-specified actions on nodes
Serialization and deserialization of the graph (for supported element types)
Provide support for polymorphic element types in nodes. Make meaningful use of STL container classes and smart pointers in the implementation of the graph class. The use of raw pointers for memory allocation and deallocation is not allowed.

Define a class Student that contains a name, surname, and student ID. Define a class Professor that contains a name, surname, and academic title. Construct a graph whose nodes contain data about individuals who can be either students or professors. Demonstrate printing (DFS order starting from an arbitrary node), serialization, and deserialization of such a graph.




