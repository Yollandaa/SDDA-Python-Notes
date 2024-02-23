# Notes
## Recap
- The index() method is similar to the find() method for strings. 
- The only difference is that find() method returns -1 if the substring is not found, whereas index() throws an exception.
- Python allows the else keyword to be used with the for and while loops too. The else block appears after the body of the loop. The statements in the else block will be executed after all iterations are completed
- movie_copy3 =  {**movie, "rating": 10, "year": 2002} 
    - The right most value replaces the left most value if the key already exists.
    - This one replaced 2001 with 2002

## Functions
- Are a way to pack your logic
```python
def sum(a, b):
    return a+b
```
- Declaration/definition -> def sum(a,b)
- Parameters/arguments -> (a,b)
- Body -> return a+b
- Why we use functions: Abstration -> You don't need to know how something works (hiding the implementation)
- Types of arguments:
    - Position arguments -> sum(1,3) -> providing it in the correct order.
    - Keyword arguments -> sum(b = 2, a = 1)
- Default values arguments should always be last and they are only used when the parameter is not provided when we call the function
- Pass by reference | library & library_list same address
    - Pass by value: Creates a copy and updates that copy
    ```python
    new_library = add_book(library.copy(), new_book)
    ```
    - Pass by reference: Updates the original library
    ```python
    print(library)
    ```
## Sets
- Sets are like lists: Mutable but only contain unique values and they don't care about order.
- Avoid using .remove() since it gives an error if the item is not present, so rather use .discard()
- Creating an empty set: new_set = set()
- use constructors: list(), set(), dict() to convert from one data type to another.

## Lamda Functions
- Lambda functions are anonymous functions: nameless function
- Should be one line
- Implicitly return (automatically)
- Use the function as temporary function, one use only. Use def if you will use the function multiple times.

```python
def fun():
    x = 4
    return x
```

- Functions are treated as first class citizen:
    - Assign a function to variable -> x = 4
    - Pass a function as argument -> fun(5)
    - Return a function -> 

```python
list = [10, 30, 60]
map(lambda x:x *2, list)
```
- This returns [20, 60, 120]. Double each value in the list array)

# What are considered false when converted to booleans
- 1. 0
- 2. None
- 3. None, False, 0.0, [], (), {}
- 4. ""

## High order function
- A function that takes another function as argument.
- E.g., map and filter

## Assignment
- Difference between parameters and arguments.
- What is currying, partials
