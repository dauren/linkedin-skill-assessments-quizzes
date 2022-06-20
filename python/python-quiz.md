## Python (Programming Language)

#### Q1. What is an abstract class?

- [ ] An abstract class is the name for any class from which you can instantiate an object.
- [ ] Abstract classes must be redefined any time an object is instantiated from them.
- [ ] Abstract classes must inherit from concrete classes.
- [x] An abstract class exists only so that other "concrete" classes can inherit from the abstract class.

[reference](https://www.geeksforgeeks.org/abstract-classes-in-python/)

#### Q2. What happens when you use the build-in function `any()` on a list?

- [ ] The `any()` function will randomly return any item from the list.
- [x] The `any()` function returns True if any item in the list evaluates to True. Otherwise, it returns False.
- [ ] The `any()` function takes as arguments the list to check inside, and the item to check for. If "any" of the items in the list match the item to check for, the function returns True.
- [ ] The `any()` function returns a Boolean value that answers the question "Are there any items in this list?"

**example**

```python
if any([True, False, False, False]) == True:
    print('Yes, there is True')
>>> 'Yes, there is True'
```

#### Q3. What data structure does a binary tree degenerate to if it isn't balanced properly?

- [x] linked list
- [ ] queue
- [ ] set
- [ ] OrderedDict

#### Q4. What statement about static methods is true?

- [ ] Static methods are called static because they always return `None`.
- [ ] Static methods can be bound to either a class or an instance of a class.
- [x] Static methods serve mostly as utility methods or helper methods, since they can't access or modify a class's state.
- [ ] Static methods can access and modify the state of a class or an instance of a class.

[reference](https://www.geeksforgeeks.org/class-method-vs-static-method-python)

#### Q5. What are attributes?

- [ ] Attributes are long-form version of an `if/else` statement, used when testing for equality between objects.
- [x] Attributes are a way to hold data or describe a state for a class or an instance of a class.
- [ ] Attributes are strings that describe characteristics of a class.
- [ ] Function arguments are called "attributes" in the context of class methods and instance methods.

**Explanation**
Attributes defined under the class, arguments goes under the functions. arguments usually refer as parameter, whereas attributes are the constructor of the class or an instance of a class.

#### Q6. What is the term to describe this code?

`count, fruit, price = (2, 'apple', 3.5)`

- [ ] `tuple assignment`
- [x] `tuple unpacking`
- [ ] `tuple matching`
- [ ] `tuple duplication`

#### Q7. What built-in list method would you use to remove items from a list?

- [ ] `.delete()` method
- [ ] `pop(my_list)`
- [ ] `del(my_list)`
- [x] `.pop()` method

**example**

```python
my_list = [1,2,3]
my_list.pop(0)
my_list
>>>[2,3]
```

#### Q8. What is one of the most common use of Python's sys library?

- [x] to capture command-line arguments given at a file's runtime
- [ ] to connect various systems, such as connecting a web front end, an API service, a database, and a mobile app
- [ ] to take a snapshot of all the packages and libraries in your virtual environment
- [ ] to scan the health of your Python ecosystem while inside a virtual environment

#### Q9. What is the runtime of accessing a value in a dictionary by using its key?

- [ ] O(n), also called linear time.
- [ ] O(log n), also called logarithmic time.
- [ ] O(n^2), also called quadratic time.
- [x] O(1), also called constant time.

#### Q10. What is the correct syntax for defining a class called Game, if it inherits from a parent class called LogicGame?

- [x] `class Game(LogicGame): pass`
- [ ] `def Game(LogicGame): pass`
- [ ] `def Game.LogicGame(): pass`
- [ ] `class Game.LogicGame(): pass`

**Explanation:** `The parent class which is inherited is passed as an argument to the child class. Therefore, here the first option is the right answer.`


#### Q12. What built-in Python data type is commonly used to represent a stack?

- [ ] `set`
- [x] `list`
- [ ] `None`
- [ ] `dictionary`
- [ ] `You can only build a stack from scratch.`

#### Q13. What would this expression return?

```python
college_years = ['Freshman', 'Sophomore', 'Junior', 'Senior']
return list(enumerate(college_years, 2019))
```

- [ ] `[('Freshman', 2019), ('Sophomore', 2020), ('Junior', 2021), ('Senior', 2022)]`
- [ ] `[(2019, 2020, 2021, 2022), ('Freshman', 'Sophomore', 'Junior', 'Senior')]`
- [ ] `[('Freshman', 'Sophomore', 'Junior', 'Senior'), (2019, 2020, 2021, 2022)]`
- [x] `[(2019, 'Freshman'), (2020, 'Sophomore'), (2021, 'Junior'), (2022, 'Senior')]`



#### Q16. What is an instance method?

- [x] Instance methods can modify the state of an instance or the state of its parent class.
- [ ] Instance methods hold data related to the instance.
- [ ] An instance method is any class method that doesn't take any arguments.
- [ ] An instance method is a regular function that belongs to a class, but it must return `None`.

#### Q17. Which statement does NOT describe the object-oriented programming concept of encapsulation?

- [ ] It protects the data from outside interference.
- [ ] A parent class is encapsulated and no data from the parent class passes on to the child class.
- [ ] It keeps data and the methods that can manipulate that data in one place.
- [x] It only allows the data to be changed by methods.


#### Q19. What built-in Python data type is best suited for implementing a queue?

- [ ] dictionary
- [ ] set
- [ ] None. You can only build a queue from scratch.
- [x] list

#### Q20. What is the correct syntax for instantiating a new object of the type Game?

- [ ] `my_game = class.Game()`
- [ ] `my_game = class(Game)`
- [x] `my_game = Game()`
- [ ] `my_game = Game.create()`

#### Q21. What does the built-in `map()` function do?

- [ ] It creates a path from multiple values in an iterable to a single value.
- [x] It applies a function to each item in an iterable and returns the value of that function.
- [ ] It converts a complex value type into simpler value types.
- [ ] It creates a mapping between two different elements of different iterables.

**Explanation:** - The synax for `map()` function is `list(map(function,iterable))`. The simple area finder using map would be like this

```python
import math
radius = [1,2,3]
area = list(map(lambda x: round(math.pi*(x**2), 2), radius))
area
>>> [3.14, 12.57, 28.27]
```

#### Q22. If you don't explicitly return a value from a function, what happens?

- [ ] The function will return a RuntimeError if you don't return a value.
- [x] If the return keyword is absent, the function will return `None`.
- [ ] If the return keyword is absent, the function will return `True`.
- [ ] The function will enter an infinite loop because it won't know when to stop executing its code.

#### Q23. What is the purpose of the `pass` statement in Python?

- [ ] It is used to skip the `yield` statement of a generator and return a value of None.
- [x] It is a null operation used mainly as a placeholder in functions, classes, etc.
- [ ] It is used to pass control from one statement block to another.
- [ ] It is used to skip the rest of a `while` or `for loop` and return to the start of the loop.

#### Q24. What is the term used to describe items that may be passed into a function?

- [x] arguments
- [ ] paradigms
- [ ] attributes
- [ ] decorators

#### Q25. Which collection type is used to associate values with unique keys?

- [ ] `slot`
- [x] `dictionary`
- [ ] `queue`
- [ ] `sorted list`

#### Q26. When does a for loop stop iterating?

- [ ] when it encounters an infinite loop
- [ ] when it encounters an if/else statement that contains a break keyword
- [x] when it has assessed each item in the iterable it is working on or a break keyword is encountered
- [ ] when the runtime for the loop exceeds O(n^2)


#### Q28. Given the following three list, how would you create a new list that matches the desired output printed below?

```python
fruits = ['Apples', 'Oranges', 'Bananas']
quantities = [5, 3, 4]
prices = [1.50, 2.25, 0.89]

#Desired output
[('Apples', 5, 1.50),
('Oranges', 3, 2.25),
('Bananas', 4, 0.89)]
```

- [ ] <br>

```python
output = []

fruit_tuple_0 = (first[0], quantities[0], price[0])
output.append(fruit_tuple)

fruit_tuple_1 = (first[1], quantities[1], price[1])
output.append(fruit_tuple)

fruit_tuple_2 = (first[2], quantities[2], price[2])
output.append(fruit_tuple)

return output
```

- [x] <br>

```python
i = 0
output = []
for fruit in fruits:
    temp_qty = quantities[i]
    temp_price = prices[i]
    output.append((fruit, temp_qty, temp_price))
    i += 1
return output
```

- [ ] <br>

```python
groceries = zip(fruits, quantities, prices)
return groceries

>>> [
('Apples', 5, 1.50),
('Oranges', 3, 2.25),
('Bananas', 4, 0.89)
]
```

- [ ]  <br>

```python
i = 0
output = []
for fruit in fruits:
    for qty in quantities:
        for price in prices:
            output.append((fruit, qty, price))
    i += 1
return output
```

#### Q29. What happens when you use the built-in function all() on a list?

- [ ] The `all()` function returns a Boolean value that answers the question "Are all the items in this list the same?
- [ ] The `all()` function returns True if all the items in the list can be converted to strings. Otherwise, it returns False.
- [ ] The `all()` function will return all the values in the list.
- [x] The `all()` function returns True if all items in the list evaluate to True. Otherwise, it returns False.

**Explanation** - `all()` returns true if all in the list are True, see example below

```python
test = [True,False,False,False]
if all(test) is True:
    print('Yeah all are True')
else:
    print('There is an imposter')
>>> 'There is an imposter'
```

#### Q30. What is the correct syntax for calling an instance method on a class named Game?

_(Answer format may vary. Game and roll (or dice_roll) should each be called with no parameters.)_

- [x] <br>

```python
>>> dice = Game()
>>> dice.roll()
```

- [ ] <br>

```python
>>> dice = Game(self)
>>> dice.roll(self)
```

- [ ] <br>

```python
>>> dice = Game()
>>> dice.roll(self)
```

- [ ] <br>

```python
>>> dice = Game(self)
>>> dice.roll()
```

#### Q31. What is the algorithmic paradigm of quick sort?

- [ ] backtracking
- [ ] dynamic programming
- [ ] decrease and conquer
- [x] divide and conquer

#### Q32. What is runtime complexity of the list's built-in `.append()` method?

- [x] O(1), also called constant time
- [ ] O(log n), also called logarithmic time
- [ ] O(n^2), also called quadratic time
- [ ] O(n), also called linear time

#### Q33. What is key difference between a `set` and a `list`?

- [ ] A set is an ordered collection unique items. A list is an unordered collection of non-unique items.
- [ ] Elements can be retrieved from a list but they cannot be retrieved from a set.
- [ ] A set is an ordered collection of non-unique items. A list is an unordered collection of unique items.
- [x] A set is an unordered collection unique items. A list is an ordered collection of non-unique items.

#### Q34. What is the definition of abstraction as applied to object-oriented Python?

- [ ] Abstraction means that a different style of code can be used, since many details are already known to the program behind the scenes.
- [x] Abstraction means the implementation is hidden from the user, and only the relevant data or information is shown.
- [ ] Abstraction means that the data and the functionality of a class are combined into one entity.
- [ ] Abstraction means that a class can inherit from more than one parent class.

#### Q35. What does this function print?

```python
def print_alpha_nums(abc_list, num_list):
    for char in abc_list:
        for num in num_list:
            print(char, num)
    return

print_alpha_nums(['a', 'b', 'c'], [1, 2, 3])
```

- [x] <br>

```python
a 1
a 2
a 3
b 1
b 2
b 3
c 1
c 2
c 3
```

- [ ] <br>

```python
['a', 'b', 'c'], [1, 2, 3]
```

- [ ] <br>

```python
aaa
bbb
ccc
111
222
333
```

- [ ] <br>

```python
a 1 2 3
b 1 2 3
c 1 2 3
```


#### Q45. What is the proper way to write a list comprehension that represents all the keys in this dictionary?

`fruits = {'Apples': 5, 'Oranges': 3, 'Bananas': 4}`

- [ ] `fruit_names = [x in fruits.keys() for x]`
- [ ] `fruit_names = for x in fruits.keys() *`
- [x] `fruit_names = [x for x in fruits.keys()]`
- [ ] `fruit_names = x for x in fruits.keys()`

#### Q47. What statement about the class methods is true?

- [ ] A class method is a regular function that belongs to a class, but it must return None.
- [x] A class method can modify the state of the class, but they can't directly modify the state of an instance that inherits from that class.
- [ ] A class method is similar to a regular function, but a class method doesn't take any arguments.
- [ ] A class method hold all of the data for a particular class.


#### Q50. According to the PEP 8 coding style guidelines, how should constant values be named in Python?

- [ ] in camel case without using underscores to separate words -- e.g. `maxValue = 255`
- [ ] in lowercase with underscores to separate words -- e.g. `max_value = 255`
- [x] in all caps with underscores separating words -- e.g. `MAX_VALUE = 255`
- [ ] in mixed case without using underscores to separate words -- e.g. `MaxValue = 255`

#### Q51. Describe the functionality of a deque.

- [ ] A deque adds items to one side and remove items from the other side.
- [ ] A deque adds items to either or both sides, but only removes items from the top.
- [x] A deque adds items at either or both ends, and remove items at either or both ends.
- [ ] A deque adds items only to the top, but remove from either or both sides.

**Explanation** - `deque` is used to create block chanin and in that there is _first in first out_ approch, which means the last element to enter will be the first to leave.

#### Q52. What is the correct syntax for creating a variable that is bound to a set?

- [x] `my_set = {0, 'apple', 3.5}`
- [ ] `my_set = to_set(0, 'apple', 3.5)`
- [ ] `my_set = (0, 'apple', 3.5).to_set()`
- [ ] `my_set = (0, 'apple', 3.5).set()`


#### Q59. What is the runtime complexity of searching for an item in a binary search tree?

- [ ] The runtime for searching in a binary search tree is O(1) because each node acts as a key, similar to a dictionary.
- [ ] The runtime for searching in a binary search tree is O(n!) because every node must be compared to every other node.
- [x] The runtime for searching in a binary search tree is generally O(h), where h is the height of the tree.
- [ ] The runtime for searching in a binary search tree is O(n) because every node in the tree must be visited.

[explanation](https://www.geeksforgeeks.org/binary-search-tree-data-structure/)

#### Q60. Why would you use `mixin`?

- [ ] You use a `mixin` to force a function to accept an argument at runtime even if the argument wasn't included in the function's definition.
- [ ] You use a `mixin` to allow a decorator to accept keyword arguments.
- [ ] You use a `mixin` to make sure that a class's attributes and methods don't interfere with global variables and functions.
- [x] If you have many classes that all need to have the same functionality, you'd use a `mixin` to define that functionality.

[explanation](https://www.youtube.com/watch?v=zVFLBfqV-q0)

#### Q61. What is the runtime complexity of adding an item to a stack and removing an item from a stack?

- [ ] Add items to a stack in O(1) time and remove items from a stack on O(n) time.
- [x] Add items to a stack in O(1) time and remove items from a stack in O(1) time.
- [ ] Add items to a stack in O(n) time and remove items from a stack on O(1) time.
- [ ] Add items to a stack in O(n) time and remove items from a stack on O(n) time.

#### Q62. Which statement accurately describes how items are added to and removed from a stack?

- [ ] a stacks adds items to one side and removes items from the other side.
- [x] a stacks adds items to the top and removes items from the top.
- [ ] a stacks adds items to the top and removes items from anywhere in the stack.
- [ ] a stacks adds items to either end and removes items from either end.

**Explanation** Stack uses the _last in first out_ approach



#### Q67. What is a lambda function ?

- [ ] any function that makes use of scientific or mathematical constants, often represented by Greek letters in academic writing
- [ ] a function that get executed when decorators are used
- [ ] any function whose definition is contained within five lines of code or fewer
- [x] a small, anonymous function that can take any number of arguments but has only expression to evaluate

[Reference](https://www.guru99.com/python-lambda-function.html)

**Explanation:**

> The lambda notation is basically an anonymous function that can take any number of arguments with only single expression (i.e, cannot be overloaded). It has been introducted in other programming languages, such as C++ and Java. The lambda notation allows programmers to "bypass" function declaration.

#### Q68. What is the primary difference between lists and tuples?

- [ ] You can access a specific element in a list by indexing to its position, but you cannot access a specific element in a tuple unless you iterate through the tuple
- [x] Lists are mutable, meaning you can change the data that is inside them at any time. Tuples are immutable, meaning you cannot change the data that is inside them once you have created the tuple.
- [ ] Lists are immutable, meaning you cannot change the data that is inside them once you have created the list. Tuples are mutable, meaning you can change the data that is inside them at any time.
- [ ] Lists can hold several data types inside them at once, but tuples can only hold the same data type if multiple elements are present.

#### Q69. What does a generator return?

- [ ] None
- [x] An iterable object
- [ ] A linked list data structure from a non-empty list
- [ ] All the keys of the given dictionary




#### Q82. What would this recursive function print if it is called with no parameters?

```python
def count_recursive(n=1):
    if n > 3:
        return
    print(n)

    count_recursive(n + 1)
```

- [ ] <br>

```python
1
1
2
2
3
3
```

- [ ] <br>

```python
3
2
1
```

- [ ] <br>

```python
3
3
2
2
1
1
```

- [x] <br>

```python
1
2
3
```

#### Q83. In Python, when using sets, you use **\_** to calculate the intersection between two sets and **\_** to calculate the union.

- [ ] `Intersect`; `union`
- [ ] `|`; `&`
- [x] `&`; `|`
- [ ] `&&`; `||`


#### Q86. what will this command return?

```python
{x for x in range(100) if x%3 == 0}
```

- [x] a set of all the multiples of 3 less then 100
- [ ] a set of all the number from 0 to 100 multiplied by 3
- [ ] a list of all the multiples of 3 less then 100
- [ ] a set of all the multiples of 3 less then 100 excluding 0

#### Q87. What does the // operator in Python 3 allow you to do?

- [x] Perform integer division
- [ ] Perform operations on exponents
- [ ] Find the remainder of a division operation
- [ ] Perform floating point division



#### Q94. Which command will create a list from 10 down to 1? Example:

`[10,9,8,7,6,5,4,3,2,1]`

- [ ] `reversed(list(range(1,11)))`
- [ ] `list(reversed(range(1,10)))`
- [ ] `list(range(10,1,-1))`
- [x] `list(reversed(range(1,11)))`


#### Q102. What built-in Python data type can be used as a hash table?

- [ ] `set`
- [ ] `list`
- [ ] `tuple`
- [x] `dictionary`


#### Q117. This code provides the **\_** of the list of numbers.

```python
num_list = [21, 13, 19, 3, 11, 5, 18]
num_list.sort()
num_list[len(num_list) // 2]
```

- [ ] mode
- [ ] average
- [ ] mean
- [x] median


#### Q120. Which choice is an immutable data type?

- [ ] dictionnary
- [ ] list
- [ ] set
- [x] string


#### Q122. Choose the option below for which instance of the class cannot be created

- [ ] Anonymous Class
- [ ] Parent Class
- [ ] Nested Class
- [x] Abstract Class


#### Q127. Which choice is not a native numerical type in Python?

- [ ] Long
- [ ] Int
- [ ] Float
- [x] Double



