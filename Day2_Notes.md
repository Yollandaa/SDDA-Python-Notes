# Day 2 Notes:

## Recap
- UX -> User Experience
- DX -> Developer experience
- Strings are immutable -> Cannot be changed

## Continuing with Python
- Comparing with strings: "100" > "9" -> False: Lexical order, 1 comes before 9: So 9 is greater.
- DRY-> Donot Repeat Yourself: Whenever you repeat yourself there is a chance to fix yourself
- You can use logical operators to fix this
- tenory operator -> 3 operands:
    - condition if ___ else ___
- Binary operators -> >, <, ==, and, or, !=, >=. <=
- unary -> not
    - Membership operator | in operator| boolean
    - tilda -> flips the 1's and 0's of a binary representation of a number
- Binary numbers: 32-bit numbers
    - 1 -> 00000000000000000000000000000000001
    - 2 -> 00000000000000000000000000000000010
    - 3 -> 00000000000000000000000000000000011
    - 4 -> 00000000000000000000000000000000100


## String and List Methods
- .chain -> Having multiple string methods in one line, one after another.
- Strings are immutable
- Lists are mutable
- When dealing with methods always check whether they manipulate your original list or not. You could do this by printing the list.
- coppp = new_list, if I change coppp I also change the new_list since they both pointing the same memory. If you do not wanna change new_list, use new_list.copy()
- The indeces store the memory addresses of the values.
- price_list -> first item memory address
- Arrays always stored in continuous memory: 456+0, 456+1, 456+2
- Reverse an array: list_form[::-1]
- list_form[::3] -> starts at index 0 and skipping 3 characters until the end

## Loops
- We have 2 types of loops:
    - for loops
    - while loop
- Range does not include the last number: rangle(1,3) (start, end) -> 1 2
- range(1, 50, 2) (start, end, skip) -> 1 3 5 7 until 49
- range(end) -> 0 1 2
- numing = [len(ave) for ave in avengers]
    - Does not mutable the original list
    - Developer experience
    - DRY
