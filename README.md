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

#### list, tuple, set, bool, dictionary
