# Day 3 Notes

## Tuple Vs Lists
- person = ("Alex", "SA", 20)
- Tuples are immutable | Liss mutable
- For lists since they are mutable: 
    - Can use sorted() as it returns a new sorted array unlike sort()
    - print(sorted(high_rate))
- Can use enumerate in a loop to get both index and value of the list.
    - for index, val in enumerate(list):
    - enumerate returns a list of tuples


## Unpacking
- Multiple variable assignemnt
    - a = b = c = 10
    - a, b, c = 10, 20, 30
    - t1, t2, _, *t3 = [20, 30, 10, 40, 50] -> use the unpacking operator * to get the remaining values, even if it a tuple, the unpacked values are going to be a list.

## Hashmaps
- Key: Value
- Keys should be unique
- KeyError -> when trying to access a nonexistent key 
- AttributeError:
- person.get('stats', {}) -> Adds default value of empty dictionary if 'stats' key doe not exist
- Unpacking operator * -> List | ** - Dictionaries

- We write code for other developers:
    - readability -> Comments/Structure/Indentation
    - efficiency
    - understability
    - performance (but not always)
    - Mantainable
    - testability
    - documentation

- CONSTANT_CASE -> when we know that variable won't change
<img src = 'https://img.brainkart.com/imagebk36/5QIE7ty.jpg'/>