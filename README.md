# Python Practice Questions & Answers

## Write short notes on the following:

- If-else statement, using an example to explain it.

The if…elif…else statement is used in Python for decision making.
Python if Statement Syntax
```py
if test expression:
    statement(s)
```

---

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

- Class in python				

  A class is a user-defined blueprint or prototype from which objects are created. Classes provide a means of bundling data and functionality together. Creating a new class creates a new type of object, allowing new instances of that type to be made. 
  
  To create a class, use the keyword class:
  
Example: Create a class named MyClass, with a property named x:
```py
class MyClass:
x = 5  X = 5
```
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
---

- Write a step-by-step process on how to create a database in python, store it and display it on the command-line.		

```py
# to create a database, you import sqlite3 from the library
import sqlite3
#next you create a connection to the database and store in a variable
#in the connect, directly parse the name of the database
con = sqlite3.connect ('customers.db')
#the database is automatically stored in the local computer
```
To run it locally on the computer:

1. Open the command prompt on the computer
2.	change the directory to the directory of the database file. Assuming the directory for the database file is in the Users directory.
`cd /c/users/`
3. Then run it by putting python before creating the filename 
`python database.py`
4. It has stored the python database in `customers.db`

---

- Write a program to create a database, create a table, insert records into the table, querry and fetchall the values to be displayed.

```py
#Create a cursor instance, it directs the database in creating tables
crs = con.cursor()
crs.execute ("""
                CREATE TABLE Customers (first_n TEXT, last_n TEXT, email TEXT,)
            """)
#commit and close the connection
con.commit()
con.close()

#run it at the commandline with python database.py
```

Insert Records into table:

```py
import sqlite3
con = sqlite3.connect ('customers.db')
crs = con.cursor()
crs.execute (" INSERT INTO customers VALUES ('John', 'Elder', 'johne@gmail.com')")
con.commit()
con.close()
```

To Querry & Fetchall:
```py
#to display we querry

import sqlite3
con = sqlite3.connect ('customers.db')
crs = con.cursor()
crs.execute (" SELECT * FROM customers")
crs.fetchall()
con.commit()
con.close()

print (crs.fetchall())

#run it through the command prompt
```
---

- Write a short note on loops, giving a syntax and an example of them.

A loop statement allows us to execute a statement or group of statements multiple times.
Syntax:
```py
for value in sequence:
    loop body
```

- Write a short note on while loops. Give a syntax and an example.

While loop is used to execute a block of statements repeatedly until a given a condition is satisfied. And when the condition becomes false, the line immediately after the loop in program is executed. 
Syntax :
```py
while expression:
    statement(s)
```
---

- Write a short note on user-defined functions		

A function is a collection of instructions. User-defined functions are codes or instructions that have been programmed and stored by the user for the purpose of calling it up. A user-defined function can also be used as a mapping.
An example of a user-defined function:
```py
def function1 ():
    print (“Lyrics one”)
    print (“Lyrics two”)
print (“This is outside the function”)
#to call up the function
print (function1 ())
```
```OUTPUT:
Lyrics one
Lyrics two
```
---

- Define dictionaries. Give a SYNTAX and an EXAMPLE.        
               
A dictionary is a lookup table used to store data values in `key:value` pairs. Dictionaries are written with curly brackets, and have keys and values:
```py
d = {key : value}
```
For example:
Create and print a dictionary:
```py
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
```
```OUTPUT
{'brand': 'Ford', 'model': 'Mustang', 'year': 1964}
```

---

- What is list slicing and manipulation? Give an example of list slicing.

Slices are good for getting a subset of values in your list. For the example code below, it will return a list with the items from index 0 up to and not including index 2.

| z= | [3, | 7, | 4, | 2] |
| -- | -- | -- | -- | -- |
| index | 0 | 1 | 2 | 3 |

First index is inclusive (before the :) and last (after the :) is not

```py
# Define a list
z = [3, 7, 4, 2]
#slice to get between the 0th index and index before the 2nd
print(z[0:2])
```
```OUTPUT
[3, 7]
```



