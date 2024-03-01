## Q1. Data Sorting and Ranking
**Objective:** Sort a complex data structure and add a ranking key based on a specific criterion.
```python
# Setup Code
students = [
    {"name": "Alice", "grade": 88},
    {"name": "Bob", "grade": 75},
    {"name": "Charlie", "grade": 93}
]
# Expected Task: Sort the list of dictionaries by grade in descending order and add a "rank" key to each dictionary based on the sorting.
```
**Expected Output:** The sorted list with an additional "rank" key for each student.

## Q2. Merging Data from Two Lists
**Objective:** Merge data from two lists of dictionaries based on a common key.
```python
# Setup Code
employees = [{"id": 1, "name": "Alice"}, {"id": 2, "name": "Bob"}]
salaries = [{"id": 1, "salary": 50000}, {"id": 2, "salary": 60000}]
# Expected Task: Merge these lists into a single list of dictionaries by matching the "id" field, including all keys.
```
**Expected Output:** A merged list of dictionaries containing both name and salary for each employee.

## Q3. Advanced Filtering with Multiple Conditions
**Objective:** Apply multiple filtering criteria to a list of dictionaries.
```python
# Setup Code
products = [
    {"id": 1, "category": "Electronics", "price": 850},
    {"id": 2, "category": "Furniture", "price": 1200},
    {"id": 3, "category": "Electronics", "price": 400}
]
# Expected Task: Filter the list to include only products in the "Electronics" category with a price less than 500.
```
**Expected Output:** A filtered list of dictionaries meeting both criteria.

## Q4. Complex Data Transformation
**Objective:** Transform a list of dictionaries into a new structure.
```python
# Setup Code
orders = [
    {"order_id": 1, "items": [{"product": "A", "quantity": 2}, {"product": "B", "quantity": 3}]},
    {"order_id": 2, "items": [{"product": "A", "quantity": 1}, {"product": "C", "quantity": 1}]}
]
# Expected Task: Transform this list into a dictionary where keys are product names and values are total quantities ordered across all orders.
```
**Expected Output:** A dictionary with product names as keys and total quantities as values.

## Q5. Data Consolidation and Summarization
**Objective:** Consolidate and summarize data from a list of dictionaries.
```python
# Setup Code
transactions = [
    {"date": "2021-01-01", "amount": 100, "category": "Food"},
    {"date": "2021-01-01", "amount": 200, "category": "Transport"},
    {"date": "2021-01-02", "amount": 150, "category": "Food"}
]
# Expected Task: Summarize the total amount spent per category.
```
**Expected Output:** A dictionary with categories as keys and total amounts spent as values.


## Q6. Grouping and Aggregating Data
**Objective:** Group data by a specific key and perform aggregation.
```python
# Setup Code
sales = [
    {"salesperson": "Alice", "amount": 200},
    {"salesperson": "Bob", "amount": 150},
    {"salesperson": "Alice", "amount": 100}
]
# Expected Task: Group sales by salesperson and calculate the total sales amount for each.
```
**Expected Output:** A dictionary with salespersons as keys and total sales amounts as values.

These assignments are designed to challenge freshers with real-world data manipulation scenarios, enhancing their problem-solving skills and proficiency in Python.


## Q7. Lambda Functions for Spell Power
**Objective:** Use a lambda function to sort a list of spells by their power level.
```python
# Setup Code
spells = [("Lumos", 5), ("Obliviate", 10), ("Expelliarmus", 7)]
# Expected Task: Sort the spells list by power level in descending order using a lambda function.
```
**Expected Output:** `[('Obliviate', 10), ('Expelliarmus', 7), ('Lumos', 5)]`


## Q8. Map Transformation for Potion Ingredients
**Objective:** Transform a list of potion ingredients to their required quantities using `map`.
```python
# Setup Code
ingredients = ["Wolfsbane", "Eye of Newt", "Dragon Scale"]
# Expected Task: Use `map` to append ": 3 grams" to each ingredient.
```
**Expected Output:** `['Wolfsbane: 3 grams', 'Eye of Newt: 3 grams', 'Dragon Scale: 3 grams']`

## Q9. Magical Book Filter and Formatter
**Objective:** Combine `filter`, `map`, and lambda functions to process a list of books and format their titles.
```python
# Setup Code
books = [{"title": "A History of Magic", "pages": 100}, {"title": "Magical Drafts and Potions", "pages": 150}]
# Expected Task: Filter books with more than 120 pages and format their titles to uppercase.
```
**Expected Output:** `['MAGICAL DRAFTS AND POTIONS']`

## Q10. Wizard Duel Game Class
**Objective:** Create a `WizardDuel` class where wizards can cast spells at each other until one wins.
```python
# Setup Code
# Expected Task: Implement a class with methods for casting spells, reducing health points, and determining the winner.
```
**Expected Output:** `After a duel between Harry and Draco, Harry wins with 10 health points left.`

## Q11. Custom Error Handling in Potion Making
**Objective:** Create a custom exception to handle errors in potion making, such as using the wrong ingredient.
```python
# Setup Code
# Expected Task: Define a `PotionError` exception and use it in a potion-making function.
```
**Expected Output:** `Caught PotionError: 'Eye of Newt' is not a valid ingredient for the Love Potion.`

## Q12. Hogwarts Library Database Query
**Objective:** Simulate a database query to find books by a specific author using list comprehensions.
```python
# Setup Code
library = [{"title": "Unfogging the Future", "author": "Cassandra Vablatsky"}, {"title": "Magical Hieroglyphs and Logograms", "author": "Bathilda Bagshot"}]
# Expected Task: Use a list comprehension to select books written by Bathilda Bagshot.
```
**Expected Output:** `[{'title': 'Magical Hieroglyphs and Logograms', 'author': 'Bathilda Bagshot'}]`

## Q13. Hogwarts House Points Calculator
**Objective:** Calculate the total points for each house using nested loops and a list of dictionaries.
```python
# Setup Code
house_points = [
    {"house": "Gryffindor", "points": 35},
    {"house": "Slytherin", "points": 50},
    {"house": "Gryffindor", "points": 60},
    {"house": "Slytherin", "points": 40}
]
# Expected Task: Aggregate points for each house and print the total.
```
**Expected Output:** `Gryffindor: 95, Slytherin: 90`

## Q14. Class Inheritance for Magical Creatures
**Objective:** Implement a class hierarchy for magical creatures where each subclass overrides a common method.
```python
# Setup Code
# Expected Task: Create a base class `MagicalCreature` and subclasses `Dragon`, `Unicorn`. Each subclass should have a unique `sound` method.
```
**Expected Output:** `Calling sound() on a Dragon instance prints 'Roar', on a Unicorn instance prints 'Neigh'.`

## Q15. Custom Sorting with Lambda for Magical Artifacts
**Objective:** Sort a list of magical artifacts by their age and power level using a custom lambda function.
```python
# Setup Code
artifacts = [
    {"name": "Cloak of Invisibility", "age": 657, "power": 9.5},
    {"name": "Elder Wand", "age": 1000, "power": 10},
    {"name": "Resurrection Stone", "age": 800, "power": 7}
]
# Expected Task: Sort the artifacts first by age, then by power, using a lambda function.
```
**Expected Output:** `Sorted list by age, then by power.`

## Q16. Wizard Profile Generator with f-strings
**Objective:** Dynamically generate wizard profiles using f-strings and dictionary unpacking.
```python
# Setup Code
wizard = {"name": "Albus Dumbledore", "title": "Headmaster", "house": "Gryffindor"}
# Expected Task: Use an f-string to create a profile string that includes the wizard's name, title, and house.
```
**Expected Output:** `'Albus Dumbledore, the Headmaster of Gryffindor.'`

## Q17. Magical Creature Adoption Matching
**Objective:** Match potential magical creature adopters with creatures based on preferences using `filter` and `map`.
```python
# Setup Code
adopters = [("Harry", "Phoenix"), ("Hermione", "House Elf")]
creatures = [("Fawkes", "Phoenix"), ("Dobby", "House Elf"), ("Buckbeak", "Hippogriff")]
# Expected Task: Use `filter` and `map` to create a list of matches between adopters and creatures.
```
**Expected Output:** `[('Harry', 'Fawkes'), ('Hermione', 'Dobby')]`

## Q18. Advanced Potion Making with Nested Loops
**Objective:** Simulate potion making where each combination of ingredients produces a unique result using nested loops.
```python
# Setup Code
ingredients = ["Moonstone", "Silver Dust", "Dragon Blood"]
# Expected Task: For each pair of ingredients, print out the unique potion they produce.
```
**Expected Output:** `Combining Moonstone and Silver Dust produces a Visibility Potion.`, etc., for all unique pairs.

## Q19. Nested Data Manipulation
**Objective:** Navigate and manipulate a nested data structure.
```python
# Setup Code
data = [
    {"id": 1, "name": "Item 1", "tags": ["tag1", "tag2"]},
    {"id": 2, "name": "Item 2", "tags": ["tag2", "tag3"]},
    {"id": 3, "name": "Item 3", "tags": ["tag1", "tag3"]}
]
# Expected Task: For each item, add a new tag "tag4" only if "tag1" is present in the tags list.
```
**Expected Output:** The original list with the modified tags list for applicable items.


## Q20. Implementing a Custom Sort Function
**Objective:** Implement a custom sort function for a list of dictionaries based on multiple criteria.
```python
# Setup Code
tasks = [
    {"id": 1, "priority": "High", "completed": False},
    {"id": 2, "priority": "Low", "completed": True},
    {"id": 3, "priority": "Medium", "completed": False}
]
# Expected Task: Sort the tasks by "completed" status (False first) and then by priority ("High", "Medium", "Low").
```
**Expected Output:** The sorted list of tasks.