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

#### list, tuple, set, bool, dictionary


## Command Line Arguments

```python
import sys

def main():
    print('Hello ', sys.argv[1])
```

