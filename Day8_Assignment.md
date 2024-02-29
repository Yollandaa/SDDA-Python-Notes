# Assignment
## 1. @property,  @balance.setter
- A property is a unique attribute that enables you to specify a method for setting or getting a class attribute's value.
-  It provides a way to access or modify the value of an attribute in a controlled manner while hiding the implementation details.
- To create a property you use the @property decorator to define a getter method for the attribute and the @<attribute>.setter decorator to define a setter method.
- Getters and setters are useful in programming because they provide you control over who can access and modify class attributes. Before allowing inputs to be assigned to an attribute, they enable you to validate them.
- 

```python
# Using the Bank class
class Bank:
    interest_rate = 0.02
    total_no_accounts = 0

    def __init__(self, acc_no, name, balance):
        self.acc_no = acc_no
        self.name = name
        self.balance = _balance  # private variable
        Bank.total_no_accounts += 1

    @property
    def balance(self):
        return self._balance

    @balance.setter
    def balance(self, value):
        if not isinstance(value, int) or value < 0:
            raise ValueError(f"{value} is not a valid input for balance")
        self._balance = value
```

```python
# Using the Animal Class example:
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        return "Some sound"

    @property #Get method to get the animal's name
    def name(self):
        return self._name

    @name.setter #Set method to set the name of the animal
    def name(self, value):
        if not isinstance(value, str) or not value.isalpha():
            raise ValueError(f"{value} is not a valid input for name")
        name_capital = value.capitalize()
        self._name = name_capital
```
 
## 2. Creating you own decorator 
### Using Functions and classes
- A decorator is a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure. 
- They play a crucial role in enhancing or modifying the behavior of functions.
- To decorate a function with a class, we use the @ syntax followed by our class name above the function definition. 
- Following convention, we use camel case for our class name. In the class definition, define two methods — the init constructor and the magic (or dunder) call method.

```python
def uppercase_decorator(function):
    def wrapper():
        func = function()
        make_uppercase = func.upper()
        return make_uppercase

    return wrapper
# decorator function takes a function as an argument, and we shall, therefore, define a function and pass it to our decorator. 

#Instead of this 
def say_hi():
    return 'hello there'

decorate = uppercase_decorator(say_hi)
decorate()

# We can change to this

@uppercase_decorator
def say_hi():
    return 'hello there'

say_hi()


```


## References
- P. (2023, March 2). Understanding Property in Python: Getters and Setters. Medium. https://medium.com/@pijpijani/understanding-property-in-python-getters-and-setters-b65b0eee62f9
- Mwiti, D. (2024, January 11). Python Decorators Tutorial. https://www.datacamp.com/tutorial/decorators-python

 