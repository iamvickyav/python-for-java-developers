# Python for Java Developers

I am a Java developer for most of my career. I started learning Python in recent months. This repo is just a recording of all my Python learning

**What is Python other than the nonvenomous snakes 🐍 found in Africa?**

* Python is a scripting language with support for Object Oriented Programming. In Java, nothing can reside outside the Class. But in Python, there is no such restriction

> Python Installation is beyond scope of this document. Please follow instructions given [here](https://www.python.org/downloads/)

## Lets Begin

### Hello World

Learning a Programming language should start with the customary printing of "Hello World". 

Imagine the horrors we gone through while explaining how to write a Hello World Program to a Java Beginner

```java
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!"); 
    }
}
```

In Python, its a breeze

```python
print("Hello World");
```

Save the above line in main.py & run the command `python main.py`. Thats it !!!

### Data Types

Here are the data types supported in Python

#### int, float, complex

Unlike Java, `int` & `float` can accommodate all whole numbers & fractional numbers respectively in Python. Remember Java has `long` & `double` types separately to handle large values

Python also has inbuilt support for `complex` numbers. The imaginary part is written with a **j suffix**. 
E.g. `c = 1 + 4j`

#### string

In Python, Strings is arrays of bytes representing unicode characters. Its case-sensitive 

Unlike Java, there is no `char` data type to store a single character

**Creating String**

Single Quote & Double Quote both can be used to create String

 `name = "Vicky"`
 `name = 'Vicky'`

To create Multiline String, use triple quotes

 ```python
 name = """My Name is Vicky. 
 I am an Indian """
 ```

**Accessing Characters in String**

In Java, we need to explicitly convert String to Char Array

```java
public class Main {
  
    public static void main(String args[])
    {
        String name = "Vicky";
        char[] ch = name.toCharArray();
  
        for (char c : ch) {
            System.out.println(c);
        }
    }
}
```

In Python, String can be iterated directly using `in` keyword

```python
name = "Vicky"
for x in name:
    print(x)
```

**Finding length of String**

use in-built len() function to find length of String

```python
name = "Vicky" 
print(len(name))
```

#### Variable Assignment in Python

In java, we can declare multiple variables in one line but we can't assign values to more than one variable at a time

**Valid Java Assignments**

```java
// Possible assignments in Java
int a, b = 10;

int a, b = 10, c;

int a=20, b=10, c=30;
```

But in Python, multiple assignments are possible


```python
# Assignment in Python
a = b = c = 10
print(a + b + c) # will print 30

a = 20
b = 30
a,b = b, a
print(a) # will print 30
print(b) # will print 20
```

Python can also unpack list/set/tuple of values to variables

```python
# Unpacking in Python
a, b, c = [1, 2, 3]
print(a) # will print 1
print(b) # will print 2
print(b) # will print 3
```

Remember, `the number of values in list should match the number of variables in left side`. Otherwise, it will throw Error

```python
# Unpacking in Python
a, b, c = [1, 2, 3, 4]
# ValueError: too many values to unpack
```

#### list, tuple, set, dictionary

Python has following inbuilt container datatypes - list, tuple, set, dictionary

| container type    | definition                        | initialization    |
|-------------------|-----------------------------------|-------------------|
| list              | mutable sequence of data in insertion order. Can access data with index        | [] or [1,2,3]     |
| set               | unordered collection of unique data                   | set()  {1, 2, 3}  |
| tuple             | immutable sequence of data in insertion order         | ()     (1,5,7)           |
| dict              | like Map in java. Key-Value pair data structure          | {}  {'name' :'Vicky', 'city': 'Chennai}              |

* `len` in-built function can take any container & returns number of items in the container
*  in operator will check whether given item exist in the container


## Operators

**Frequently used Operators** for reference

| Operator  | Operation  |
|-----------|------------|
| x+y, x-y  | Addition, Subtraction  | 
| x*y       | Multiplication  |
| x/y       | Float Division        |
| x//y      | Integer Division      |
| x%y       | Remainder of Integer Division      |
| x ** y    | x power y |
| and       | BOOLEAN AND operator (used in IF condition) |
| or        | BOOLEAN OR operator (used in IF condition) |
| not       | BOOLEAN NOT operator |
| x is y, x is not y    | Checking whether objects refering to same instance |
| x in y, x not in y    | Check if x is part of y |

In java, If we want to check two conditions, we separate them with `&&`, `||` operators. 

In python, we can combine multiple conditions

```java
// Multiple Condition in Java
a<b && b<c && c>d

// Multiple Condition in Python
a < b < c > d
```

```python
// Multiple Condition in Python Sample
a= 10
b = 20
c = 30
d = 40

print(a < b < c < d) # prints True
```

**Ternary Operator**

In Java, the syntax is as follow

`CONDITION ? RETURNVALUEFORTRUE: RETURENVALUEFORFALSE`

In python, the syntax is as follow

`RETURNVALUEFORTRUE if CONDITION else RETURENVALUEFORFALSE`

```java
# Ternary Operator in Java
String gender = "Female";
String salutation = gender.equals("Male") ? "Mr" : "Mrs";
System.out.println(salutation); # prints Mrs
```

```python
# Ternary Operator in Python
gender = 'Female'

print('Mr' if gender == "Male" else 'Mrs') # Mrs

gender = 'Male'

print('Mr' if gender == "Male" else 'Mrs') # Mr
```

## Command Line Arguments

```python
import sys

def main():
    print('Hello ', sys.argv[1])
```


## To read
* General Purpose Special Methods
* Container Methods
