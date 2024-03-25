# learn-python
This repository is used for learning python and contains basic concepts and resources for revision in future.
  
   STARTING - 
1.
Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.
It is used for:
web development (server-side),
software development,
mathematics,
system scripting.

2.
Indentation refers to the spaces at the beginning of a code line.(the free space before the "print")
if 5 > 2:
  print("Five is greater than two!")

3.
VARIABLES
Python has no command for declaring a variable.
A variable0 is created the moment you first assign a value to it.
 11
   1.. specifying the data type of variable is called as casting
       x = str(3)
       y = int(3)
       z = float(3)

             print(x)
             print(y)
             print(z)

    2.. You can get the data type of a variable with the type() function.
        x = 5
        y = "John"
        print(type(x))
        print(type(y))

    3.. Variable names are case-sensitive.
          A and a are different

    4.. String variables can be declared either by using single or double quotes.
   
  22 
    1.. Camel Case - 
           Each word, except the first, starts with a capital letter
        myVariableName = "John"

    2.. Pascal Case - 
           Each word starts with a capital letter
        MyVariableName = "John"

    3.. Snake Case - 
           Each word is separated by an underscore character
        my_variable_name = "John"
 
  33
    1.. Many Values to Multiple Variables - 
        Python allows you to assign values to multiple variables in one line:
        Many Values to Multiple Variables
        x, y, z = "Orange", "Banana", "Cherry"
        print(x)
        print(y)
        print(z)

    2.. Unpack a Collection - 
        If you have a collection of values in a list, tuple etc. Python allows you to extract the values into variables. This is called unpacking.
        fruits = ["apple", "banana", "cherry"]
        x, y, z = fruits
        print(x)
        print(y)
        print(z)
    
  44
    1.. Global Variables - 
        ariables that are created outside of a function (as in all of the examples above) are known as global variables.
        Global variables can be used by everyone, both inside of functions and outside.
        x = "awesome"

        def myfunc():
          print("Python is " + x)
        
        myfunc()

    2.. The global Keyword -
        Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
        To create a global variable inside a function, you can use the global keyword.
        def myfunc():
         global x
            x = "fantastic"

         myfunc()

         print("Python is " + x)

4.
Multiline Comments
#This is a comment
#written in
#more than just one line
print("Hello, World!") 
              OR
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!") 

5.
  Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	    set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	    NoneType

Example	Data Type	Try it
x = "Hello World"	str	
x = 20	int	
x = 20.5	float	
x = 1j	complex	
x = ["apple", "banana", "cherry"]	list	
x = ("apple", "banana", "cherry")	tuple	
x = range(6)	range	
x = {"name" : "John", "age" : 36}	dict	
x = {"apple", "banana", "cherry"}	set	
x = frozenset({"apple", "banana", "cherry"})	frozenset	
x = True	bool	
x = b"Hello"	bytes	
x = bytearray(5)	bytearray	
x = memoryview(bytes(5))	memoryview	
x = None	NoneType	
Setting the Specific Data Type
If you want to specify the data type, you can use the following constructor functions:

Example	                                                       Data Type
x = str("Hello World")	                                       str	
x = int(20)	                                                   int	
x = float(20.5)	                                               float	
x = complex(1j)	                                               complex	
x = list(("apple", "banana", "cherry"))	                       list	
x = tuple(("apple", "banana", "cherry"))	                   tuple	
x = range(6)                                                   range	
x = dict(name="John", age=36)	                               dict	
x = set(("apple", "banana", "cherry"))	                       set	
x = frozenset(("apple", "banana", "cherry"))	               frozenset	
x = bool(5)	                                                   bool	
x = bytes(5)	                                               bytes	
x = bytearray(5)	                                           bytearray	
x = memoryview(bytes(5))	                                   memoryview

6.


25/03/24
Python supports the usual logical conditions from mathematics:

Equals: a == b
Not Equals: a != b
Less than: a < b
Less than or equal to: a <= b
Greater than: a > b
Greater than or equal to: a >= b


Elif
The elif keyword is Python's way of saying "if the previous conditions were not true, then try this condition".
ex-
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
                In this example a is equal to b, so the first condition is not true, but the elif condition is true, so we print to screen that "a and b are equal".

and lastly the "else" - it is the last option, it should not any condtion.
if no above condition in code is satisfied then this "else" works.
ex-
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")

ultimately the conclusion is, "if" and "elif" can have conditions but not "else"

Short Hand If ... Else
If you have only one statement to execute, one for if, and one for else, you can put it all on the same line:
ex-
a = 2
b = 330
print("A") if a > b else print("B")

Nested If
You can have if statements inside if statements, this is called nested if statements.
ex- 
x = 41

if x > 10:
  print("Above ten,")
  if x > 20:
    print("and also above 20!")
  else:
    print("but not above 20.")

The while Loop
With the while loop we can execute a set of statements as long as a condition is true.
