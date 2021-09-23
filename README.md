# Python Practice Questions & Answers

- Decorators in Python?

Decorators are used to add some design patterns to a function without changing its structure. Decorators generally are defined before the function they are enhancing. To apply a decorator we first define the decorator function. Then we write the function it is applied to and simply add the decorator function above the function it has to be applied to. For this, we use the @ symbol before the decorator.

--- 

- Constructor in Python
  
Constructors are generally used for instantiating an object. The task of constructors is to initialize(assign values) to the data members of the class when an object of the class is created. In Python the __init__() method is called the constructor and is always called when an object is created.

--- 

- Inheritance in Python
  
Inheritance allows us to define a class that inherits all the methods and properties from another class.
Parent class is the class being inherited from, also called base class.
Child class is the class that inherits from another class, also called derived class.

--- 

- Object in python

  An Object is an instance of a Class. A class is like a blueprint while an instance is a copy of the class with actual values.
Now we can use the class named MyClass to create objects:


Example:  Create an object named p1, and print the value of x:
```py 
p1 = MyClass()
print(p1.x)
```
--- 
- Class in python				

  A class is a user-defined blueprint or prototype from which objects are created. Classes provide a means of bundling data and functionality together. Creating a new class creates a new type of object, allowing new instances of that type to be made. 
  
  To create a class, use the keyword class:
  
Example: Create a class named MyClass, with a property named x:
```py
class MyClass:
x = 5  X = 5
```
--- 

- List 5 Differences between lists and tuples


| List                                                         |Tuples                                                        | 
|--------------------------------------------------------------|--------------------------------------------------------------|
|Lists are mutable                                             |Tuples are immutable                                          |
|Implication of iterations is Time-consuming                   |The implication of iterations is comparatively Faster         |
|The list is better for performing operations, such as insertion and deletion.|Tuple data type is appropriate for accessing the elements|
|Lists consume more memory|Tuple consume less memory as compared to the list|
|Lists have several built-in methods|Tuple does not have many built-in methods.|
|The unexpected changes and errors are more likely to occur|In tuple, it is hard to take place.|

--- 

- List three similarities between lists and tuples

1. Lists and Tuples are ordered. They can be accessed by indexing
2. Lists and Tuples can hold duplicate values.
3. Lists and Tuples can hold mutable objects like lists.

---

- Dict and List comprehensions in Python?

Dictionary and list comprehensions are just another concise way to define dictionaries and lists.

Example of list comprehension is-

```py 
x = [i for i in range(5)]
```

The above code creates a list as below-

```py
4
[0,1,2,3,4]
```

Example of dictionary comprehension is-

```py
x = [i : i+2 for i in range(5)]
```
The above code creates a list as below-

```py
[0: 2, 1: 3, 2: 4, 3: 5, 4: 6]
```
