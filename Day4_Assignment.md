# Assignment
## Difference between parameters and arguments.
- From a function's perspective we can define a parameter as the variable listed inside the parantheses in the function definition.
- From the code below: a and b inside the paranthesis are the parameters.

- While an argument is the value that is sent to the function when you do a function call.
- Using the same code: The arguments are 3 and 4 in the print statement.

```python
def sum(a, b):
    return a+b
print(f"The sum is {sum(3,4)}")
```

<img src = 'https://www.baeldung.com/wp-content/ql-cache/quicklatex.com-758a1e9312a5c906adf2b86103b12c06_l3.svg'/>


## What is currying, partials
- Currying is the transformation of a function with multiple arguments into a sequence of single-argument functions. That means converting a function like this sum(a, b, c) into a function like this sum(a)(b)(c)
- currying requires functions to have a fixed number of arguments. 
- Curry also produces a higher order function: any function that takes a function as at least one of its parameters or returns a function as its result.
- To evaluate this, we take the sum function and curry it.
```python
def curry_sum(a):
    def inner(b):
        return a+b
    return inner
print(curry_sum(3)(4))
```

- Partial functions help in deriving a function with n parameters to a function with fewer parameters.
-  We take a function that has some number of arguments and we fix some of those arguments to a set value. We then return a function that has less arguments than the original. This function with fixed arguments can then be called from anywhere else in the code and it will be as if we had called the original function with all of its arguments. 
- You can use partial functions if there is a function that we use often in the code where one or more of the arguments that we call with is almost always the same. Also helps in reducing duplication and helps in code reusability.


```python
   
from functools import *
# A normal function
def add(a, b, c):
    return  a + b + c
 
# A partial function with b = 1 and c = 2
add_part = partial(add, c = 2, b = 1)
 
# Calling partial function
print(add_part(3))
```

## References
- Python Function Arguments. (n.d.). https://www.w3schools.com/python/gloss_python_function_arguments.asp#:~:text=A%20parameter%20is%20the%20variable,function%20when%20it%20is%20called.

- Science, B. O. C., & Science, B. O. C. (2022, September 29). The Difference Between an Argument and a Parameter | Baeldung on Computer Science. Baeldung on Computer Science. https://www.baeldung.com/cs/argument-vs-parameter

- Himite, B. (2022, January 5). What Is Currying in Programming? - Towards Data Science. Medium. https://towardsdatascience.com/what-is-currying-in-programming-56fd57103431

- G. (2023, August 21). Partial Functions in Python. GeeksforGeeks. https://www.geeksforgeeks.org/partial-functions-python/

