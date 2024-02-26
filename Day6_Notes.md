# Recap
- properties of map:
    - you want to change the data type 
    - mantain the length of the original one
    - it always returns a copy of the array

- properties of filter:
    - it always returns a copy of the array
    - Mantains the data type
    - Returns a shorter length of the original list
- pretty print: import pprint: 
- dunder variable: __name__: the underscores
    - when importing from another, "__name__" will be the file name, the file you are importing
- Variable names:
    - Should not be keywords -> for, class
    - Case-sensitive -> city, CITY
    - no special signs -> except underscore
    - can not start with a number
- Rename a variable: F2 or "ctrl + d"
- curly brackets is called interpollation

```python
# Nested comprehensions
class_avg = {class_name: get_avg([get_avg(student['grades']) for student in students]) for class_name, students in classes.items() }
pprint(class_avg)
```

# Regex
- Regex is case-sensitive: to avoid this, use flags=re.IGNORECASE
- \d\d\d: Anything from 0-9
- \D: Anything that is not a digit
- .: Anything will match
- \s: Anything that is a space
- - ..: Anything that is not a space
-  \.: Exactly 
- [abc]d: Anything that is a, b, or c, and it should have d after
- [^abcs]: Anything that is not a, b, or c
- [a-z]: Anything that is a-z ( from a to z)
- \w ==  [A-Za-z0-9_]: Anything that is a-z, 0-9, or _ (Alphanumeric)
- \W: Anything that is not a-z, 0-9, or _ 
- {w}: Exactly w times (repetition)
- n+ : One or more
- *: Zero or more times
ab?c:  will match either the strings "abc" or "ac" because the b is considered optional.
-  [^...]: Anything that is not ...
-  ^hat$: Matches the string "hat" at the beginning and end of the string.
- ^success: Matches the string "success" at the beginning of the string.
- success$: Matches the string "success" at the end of the string.
- ^(IMG\d+\.png)$: Matches the string "IMG123.png" at the beginning of the string.
- .*x.* : A greedy approach takes anything with x inbetween and anything after
- .*x.*? : A non-greedy approach takes anything with x inbetween and anything after.

# Using regex in Python
- import re
```python
import re
quote = "To be or not to be"
is_be = re.search(r'be$', quote)
output = "Present" if is_be else "Not present"
print(is_be, type(is_be))
print(output)
```

```python
# Output
#['#sunny', '#California', '#travel', '#fun']
# Get the words with the hashtags

post = "Loving the #sunny weather in #California. #travel #fun"
hashtags = re.findall(r'#\w+', post)
print(hashtags)
```
