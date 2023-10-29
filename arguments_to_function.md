# args vs kwargs in Python

```python
def order_ice_cream(size, flavour, *toppings, **details):
    print(f'You have ordered {size} size {flavour} ice cream with toppings {toppings}')
    print(f'Your order details are as follow {details}')


if __name__ == '__main__':
    order_ice_cream('Small', "Choco", "Cherry", "Sprinkles", address="Chennai", COD=True)
    

# Output
# You have ordered Small size Choco ice cream with toppings ('Cherry', 'Sprinkles')
# Your order details are as follow {'address': 'Chennai', 'COD': True}
```

`*toppings` - collects all non keyworded arguments, in this case, ` "Choco", "Cherry", "Sprinkles"` - arguments are converted to tuples

`**details` - collects all keyworded arguments, in this case, `address="Chennai", COD=True` - arguments are converted to dictionary



