# Generators in Python

Here are few sample generators

## range()

range() returns an **iterable** object which returns the successive items of the desired sequence when you iterate over it. 

```python
print(range(10))

# Output
# range(0, 10)
```

```python
for i in range(5):
    print(x, end=" ")

# Output
# 0 1 2 3 4

for x in range(1, 11):
    print(x, end=" ")

# Output
# 1 2 3 4 5 6 7 8 9 10 

for x in range(0, 10, 3):
    print(x, end=" ")

# Output
# 0 3 6 9 

for x in range(-10, -100, -30):
    print(x, end=' ')

# Output
# -10 -40 -70
```