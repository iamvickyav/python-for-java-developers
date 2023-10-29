# List Comprehension

```python
names = ['vicky', 'vijay', 'vaishu']

length_of_names = [len(name) for name in names]
print(length_of_names)

# [5, 5, 6]
```

## Set comprehension

```python
names = ['vicky', 'vijay', 'vaishu']

length_of_each_name = {name: len(name) for name in names}
print(length_of_each_name)

{'vicky': 5, 'vijay': 5, 'vaishu': 6}
```
