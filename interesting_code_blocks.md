# Interesting Code Blocks

## Fibonacci Series 

```python
def fib(n):
    a, b = 0, 1
    while a < n:
        print(a, end=' ')
        a, b = b, a+b
    print()
```

## char to int

```python
ord('a')
# Will print 97
```

## else block is possible for for loop

a try statement’s else clause runs when no exception occurs, and a loop’s else clause runs when no break occurs

```python
for i in range(10):
    if i > 10:
        break
else:
    print('no number is greater than 10 in given range')
```

## match aka switch with class (supported only in Python 3.10)

```python
class Point:
    x: int
    y: int
    
    def __init__(self, x, y):
        self.x = x
        self.y = y

def where_is(point):
    match point:
        case Point(x=0, y=0):
            print("Origin")
        case Point(x=0, y=y):
            print(f"Y={y}")
        case Point(x=x, y=0):
            print(f"X={x}")
        case Point():
            print("Somewhere else")
        case _:
            print("Not a point")

where_is(Point(10, 0))
```

## Create Constructor automatically

```python
from dataclasses import dataclass

@dataclass
class Point:
    x: int
    y: int
    
    # def __init__(self, x, y):
    #     self.x = x
    #     self.y = y
```

## Function arguments with * and **

* in argument means tuples
** in argument means dict

```python
def concat(*args, sep="/"):
    return sep.join(args)

concat("earth", "mars", "venus")
```

## unpack args

*-operator to unpack the arguments out of a list or tuple
** - unpack the arguments out of a dict

```python
args = [3, 6]
list(range(*args)) 
```

```python
def parrot(voltage, state='a stiff', action='voom'):
    pass

d = {"voltage": "four million", "state": "bleedin' demised", "action": "VOOM"}
parrot(**d)
```

## prime numbers in a range

```python
nums = range(1, 1000)


def is_prime(num):
    for x in range(2, num):
        if (num % x) == 0:
            return False
    return True


primes = list(filter(is_prime, nums))
print(primes)
```
