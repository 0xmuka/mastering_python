## Lists

1. **Creating Lists:**
    - Lists are created by enclosing elements within square brackets `[ ]`, separated by commas.
    
    ```python
    # Creating a list of integers
    my_list = [1, 2, 3, 4, 5]
    
    # Creating a list of strings
    fruits = ['apple', 'banana', 'orange', 'kiwi']
    
    # Creating a list of mixed data types
    mixed_list = [1, 'apple', True, 3.14]
    
    ```
    
2. **Accessing Elements:**
    - You can access individual elements of a list using indexing.
    
    ```python
    # Accessing the first element
    first_element = my_list[0]
    
    # Accessing the last element
    last_element = my_list[-1]
    
    ```
    
3. **Slicing Lists:**
    - You can create a sublist (slice) of a list using slicing notation `[start:end:step]`.
    
    ```python
    # Getting a sublist from index 1 to 3
    sublist = my_list[1:4]
    
    # Getting a sublist from index 0 to 3 with step 2
    sliced_list = my_list[0:4:2]
    
    ```
    
4. **Modifying Lists:**
    - Lists are mutable, so you can modify their elements or change the list's structure after creation.
    
    ```python
    # Modifying an element
    my_list[2] = 10
    
    # Appending an element to the end
    my_list.append(6)
    
    # Removing an element by value
    my_list.remove(4)
    
    ```
    
5. **List Methods:**
    - Python provides various built-in methods to manipulate lists.
    
    ```python
    # Appending elements
    fruits.append('grape')
    
    # Inserting an element at a specific index
    fruits.insert(1, 'pear')
    
    # Removing an element by index
    fruits.pop(2)
    
    # Extending the list with another list
    fruits.extend(['pineapple', 'mango'])
    
    # Sorting the list
    fruits.sort()
    
    # Reversing the list
    fruits.reverse()
    
    ```
    
6. **Iterating Over Lists:**
    - You can iterate over the elements of a list using loops or list comprehensions.
    
    ```python
    # Using a for loop
    for fruit in fruits:
        print(fruit)
    
    # Using list comprehension
    upper_fruits = [fruit.upper() for fruit in fruits]
    
    ```
    

These examples illustrate various operations you can perform with lists in Python, from creating and accessing elements to modifying lists and using list methods. Lists are versatile data structures that are widely used in Python programming for storing and manipulating collections of items.

## Accessing Items

Accessing items in a list is done using indexing. In Python, indexing starts from 0, meaning the first element of a list has an index of 0, the second element has an index of 1, and so on. You can also use negative indices to access elements from the end of the list, with -1 representing the last element, -2 representing the second-to-last element, and so forth.

Here are some examples demonstrating how to access items in a list:

```python
# Define a list
my_list = ['apple', 'banana', 'orange', 'kiwi', 'grape']

# Access the first item
first_item = my_list[0]
print("First item:", first_item)  # Output: apple

# Access the last item
last_item = my_list[-1]
print("Last item:", last_item)  # Output: grape

# Accessing items in a sublist
sublist = my_list[1:4]
print("Sublist:", sublist)  # Output: ['banana', 'orange', 'kiwi']

# Accessing every other item
every_other = my_list[::2]
print("Every other item:", every_other)  # Output: ['apple', 'orange', 'grape']

```

In these examples:

- `my_list[0]` accesses the first item in the list.
- `my_list[-1]` accesses the last item in the list.
- `my_list[1:4]` accesses a sublist containing items from index 1 to 3.
- `my_list[::2]` accesses every other item in the list.

You can also use list slicing to access multiple items at once or to create a new list containing a subset of the original list. Understanding how to access items in a list is fundamental to working with lists effectively in Python.

## List unpacking

List unpacking, also known as iterable unpacking, is a feature in Python that allows you to extract the elements of a list (or any iterable) and assign them to individual variables in a single statement. This is particularly useful when you have a list with known structure or length and you want to assign its elements to separate variables without having to access them individually using indexing.

Here's how list unpacking works in Python:

```python
# Define a list
my_list = [1, 2, 3]

# Unpack the list into individual variables
a, b, c = my_list

# Print the values of the variables
print("a:", a)  # Output: 1
print("b:", b)  # Output: 2
print("c:", c)  # Output: 3

```

In this example:

- The elements of `my_list` are unpacked into individual variables `a`, `b`, and `c`.
- Each variable receives the corresponding value from the list.
- You can then use these variables independently in your code.

List unpacking can also be used with extended iterable unpacking using the `*` operator to capture multiple values into a single variable:

```python
# Define a list
my_list = [1, 2, 3, 4, 5]

# Unpack the first and last elements, and capture the rest in a variable
first, *middle, last = my_list

# Print the values of the variables
print("first:", first)    # Output: 1
print("middle:", middle)  # Output: [2, 3, 4]
print("last:", last)      # Output: 5

```

In this example, `*middle` captures all elements between the first and last elements into a list. This is useful when you want to process parts of a list separately while keeping the remaining elements intact.

List unpacking provides a concise and readable way to work with lists in Python, especially when dealing with collections of known size or structure.

## Looping over lists

Looping over lists in Python is quite straightforward using a `for` loop. Here's a simple example:

```python
# Define a list of numbers
numbers = [1, 2, 3, 4, 5]

# Loop over each number in the list
for number in numbers:
    print(number)

```

Output:

```
1
2
3
4
5

```

In this example:

- We define a list called `numbers` containing integers from 1 to 5.
- We use a `for` loop to iterate over each element (`number`) in the list.
- Inside the loop, we print each `number`.

This loop will iterate over each item in the list sequentially, executing the indented block of code (in this case, `print(number)`) for each iteration. It's a simple and common way to process each element of a list in Python.

## Adding or removing elements

Adding or removing elements from a list in Python is a common operation, and Python provides several methods for modifying lists dynamically. Here are some common ways to add or remove elements from a list:

1. **Appending Elements:**
    - The `append()` method adds a single element to the end of the list.
    
    ```python
    my_list = [1, 2, 3]
    my_list.append(4)
    print(my_list)  # Output: [1, 2, 3, 4]
    
    ```
    
2. **Extending Lists:**
    - The `extend()` method adds all the elements of another list to the end of the current list.
    
    ```python
    my_list = [1, 2, 3]
    my_list.extend([4, 5, 6])
    print(my_list)  # Output: [1, 2, 3, 4, 5, 6]
    
    ```
    
3. **Inserting Elements:**
    - The `insert()` method inserts an element at a specified position in the list.
    
    ```python
    my_list = [1, 2, 3]
    my_list.insert(1, 'a')
    print(my_list)  # Output: [1, 'a', 2, 3]
    
    ```
    
4. **Removing Elements:**
    - The `remove()` method removes the first occurrence of a specified value from the list.
    
    ```python
    my_list = [1, 2, 3, 2]
    my_list.remove(2)
    print(my_list)  # Output: [1, 3, 2]
    
    ```
    
5. **Popping Elements:**
    - The `pop()` method removes and returns the element at a specified index. If no index is provided, it removes and returns the last element.
    
    ```python
    my_list = [1, 2, 3]
    popped_element = my_list.pop(1)
    print(popped_element)  # Output: 2
    
    ```
    
6. **Clearing the List:**
    - The `clear()` method removes all elements from the list, leaving it empty.
    
    ```python
    my_list = [1, 2, 3]
    my_list.clear()
    print(my_list)  # Output: []
    
    ```
    

These methods provide flexibility for modifying lists dynamically, allowing you to add, remove, or modify elements as needed.

## Finding items

Finding items in a list in Python can be done using various methods. Here are some common approaches:

1. **Using the `in` Operator:**
    - The `in` operator checks if an element exists in a list.
    
    ```python
    my_list = [1, 2, 3, 4, 5]
    if 3 in my_list:
        print("3 is in the list")
    
    ```
    
2. **Using the `index()` Method:**
    - The `index()` method returns the index of the first occurrence of a specified value in the list. If the value is not found, it raises a `ValueError`.
    
    ```python
    my_list = [1, 2, 3, 4, 5]
    index = my_list.index(3)
    print("Index of 3:", index)  # Output: 2
    
    ```
    
3. **Using a Loop:**
    - You can iterate over the list using a loop and check each element manually.
    
    ```python
    my_list = [1, 2, 3, 4, 5]
    for item in my_list:
        if item == 3:
            print("3 is in the list")
            break
    
    ```
    
4. **Using the `count()` Method:**
    - The `count()` method returns the number of occurrences of a specified value in the list.
    
    ```python
    my_list = [1, 2, 3, 3, 4, 5]
    count = my_list.count(3)
    print("Number of occurrences of 3:", count)  # Output: 2
    
    ```
    
5. **Using List Comprehension:**
    - You can use list comprehension to filter elements that match a certain condition.
    
    ```python
    my_list = [1, 2, 3, 4, 5]
    found = [item for item in my_list if item == 3]
    if found:
        print("3 is in the list")
    
    ```
    

These methods provide different ways to find items in a list in Python, allowing you to choose the one that best fits your needs and preferences.

## Sorting lists

Sorting lists in Python can be done using the `sort()` method or the `sorted()` function. The `sort()` method sorts the list in place, while the `sorted()` function returns a new sorted list without modifying the original list.

Here's how to use each method:

1. **Using the `sort()` Method:**
    - The `sort()` method sorts the list in ascending order by default. You can specify the `reverse=True` parameter to sort in descending order.
    
    ```python
    my_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
    my_list.sort()
    print("Sorted list:", my_list)
    
    ```
    
    Output:
    
    ```
    Sorted list: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]
    
    ```
    
    To sort in descending order:
    
    ```python
    my_list.sort(reverse=True)
    print("Sorted list (descending):", my_list)
    
    ```
    
    Output:
    
    ```
    Sorted list (descending): [9, 6, 5, 5, 4, 3, 3, 2, 1, 1]
    
    ```
    
2. **Using the `sorted()` Function:**
    - The `sorted()` function returns a new sorted list without modifying the original list.
    
    ```python
    my_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
    sorted_list = sorted(my_list)
    print("Original list:", my_list)
    print("Sorted list:", sorted_list)
    
    ```
    
    Output:
    
    ```
    Original list: [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
    Sorted list: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]
    
    ```
    
    To sort in descending order:
    
    ```python
    sorted_list_desc = sorted(my_list, reverse=True)
    print("Sorted list (descending):", sorted_list_desc)
    
    ```
    
    Output:
    
    ```
    Sorted list (descending): [9, 6, 5, 5, 4, 3, 3, 2, 1, 1]
    
    ```
    

Both methods allow you to sort lists in Python, providing flexibility in terms of whether you want to sort the list in place or create a new sorted list without modifying the original one.

## **Lambda Functions**

Let's compare lambda functions with normal (named) functions in Python.

**Lambda Functions:**

- Lambda functions are anonymous functions, meaning they do not have a name.
- They are defined using the `lambda` keyword followed by parameters and an expression.
- Lambda functions are typically used for short, simple operations that can be expressed in a single line of code.
- They are often used in situations where a small function is needed for a short period of time, such as when passing a function as an argument to another function.

**Normal (Named) Functions:**

- Normal functions have a name and are defined using the `def` keyword followed by the function name, parameters, and a block of code.
- They can contain multiple statements and can be of any length.
- Normal functions provide more flexibility and readability, especially for complex operations.
- They are used when you need to reuse the same functionality multiple times throughout your code or when the function logic is more complex.

**Comparison:**

- Lambda functions are more concise and are often used for short, simple operations that can be defined in a single line.
- Normal functions provide more structure and flexibility, making them suitable for complex operations or when the same functionality needs to be reused multiple times.

**Example - Lambda Function:**

```python
# Lambda function to calculate the square of a number
square = lambda x: x ** 2
print(square(5))  # Output: 25

```

**Example - Normal Function:**

```python
# Normal function to calculate the square of a number
def square(x):
    return x ** 2

print(square(5))  # Output: 25

```

In these examples, both the lambda function and the normal function achieve the same result of calculating the square of a number. However, the lambda function is more concise and does not require a function name or the `return` keyword. Normal functions, on the other hand, provide more structure and can contain multiple statements if needed.

## Map Function

The `map()` function in Python is a built-in function that applies a specified function to each item in an iterable (such as a list) and returns an iterator that yields the results. It takes two arguments: the function to apply and the iterable to apply it to. The `map()` function returns a map object, which is an iterator that yields the results of applying the function to each item in the iterable.

**Syntax:**

```python
map(function, iterable)

```

- `function`: The function to apply to each item in the iterable. This can be a built-in function, a lambda function, or any other callable.
- `iterable`: The iterable (e.g., list, tuple, etc.) whose elements will be passed to the function.

**Example:**
Suppose we have a list of numbers and we want to calculate the squares of each number using the `map()` function:

```python
numbers = [1, 2, 3, 4, 5]

# Using map with a lambda function
squared_numbers = map(lambda x: x ** 2, numbers)

# Converting the map object to a list to see the results
squared_numbers_list = list(squared_numbers)
print(squared_numbers_list)  # Output: [1, 4, 9, 16, 25]

```

In this example:

- We have a list of numbers `[1, 2, 3, 4, 5]`.
- We use the `map()` function with a lambda function `lambda x: x ** 2` to calculate the squares of each number.
- The `map()` function returns a map object, which is then converted to a list `squared_numbers_list` using the `list()` function to see the results.
- The resulting list contains the squares of each number in the original list.

The `map()` function is commonly used for applying a function to each item in an iterable, especially when the transformation is simple and can be expressed as a one-liner using a lambda function. It provides a concise and efficient way to perform the same operation on each element in a collection.

**`map()` Function with Lambda:**

```python
# Using map with a lambda function
numbers = [1, 2, 3, 4, 5]
squared_numbers = map(lambda x: x ** 2, numbers)

# Converting the map object to a list to see the results
squared_numbers_list = list(squared_numbers)
print(squared_numbers_list)  # Output: [1, 4, 9, 16, 25]

```

**Default (Named) Function:**

```python
# Defining a named function
def square(x):
    return x ** 2

# Using a loop to apply the function to each element
numbers = [1, 2, 3, 4, 5]
squared_numbers = []
for num in numbers:
    squared_numbers.append(square(num))

print(squared_numbers)  # Output: [1, 4, 9, 16, 25]

```

In these examples, both methods achieve the same result of calculating the squares of each number in the list. The `map()` function with a lambda function offers a more concise approach, while the default (named) function provides a more structured and readable solution.

## Filter Function

The `filter()` function in Python is another built-in function that is used to filter elements from an iterable (such as a list) based on a specified condition. It takes two arguments: the function that defines the filtering condition and the iterable to be filtered. The `filter()` function returns an iterator that yields only the elements from the iterable for which the function evaluates to `True`.

**Syntax:**

```python
filter(function, iterable)

```

- `function`: The function that defines the filtering condition. This function should return `True` for elements to be included in the output and `False` for elements to be excluded.
- `iterable`: The iterable (e.g., list, tuple, etc.) from which elements will be filtered.

**Example:**
Suppose we have a list of numbers and we want to filter out only the even numbers using the `filter()` function:

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Using filter with a lambda function to filter even numbers
even_numbers = filter(lambda x: x % 2 == 0, numbers)

# Converting the filter object to a list to see the results
even_numbers_list = list(even_numbers)
print(even_numbers_list)  # Output: [2, 4, 6, 8, 10]

```

In this example:

- We have a list of numbers `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`.
- We use the `filter()` function with a lambda function `lambda x: x % 2 == 0` to filter out only the even numbers.
- The `filter()` function returns a filter object, which is then converted to a list `even_numbers_list` using the `list()` function to see the results.
- The resulting list contains only the even numbers from the original list.

The `filter()` function is commonly used for filtering elements from an iterable based on a specified condition. It provides a concise and efficient way to select elements that meet certain criteria from a collection.

- Let's compare the `filter()` function with a default (named) function in Python without using list comprehensions.

**`filter()` Function with Lambda:**

```python
# Using filter with a lambda function to filter even numbers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = filter(lambda x: x % 2 == 0, numbers)

# Converting the filter object to a list to see the results
even_numbers_list = list(even_numbers)
print(even_numbers_list)  # Output: [2, 4, 6, 8, 10]

```

**Default (Named) Function:**

```python
# Defining a named function to check if a number is even
def is_even(x):
    return x % 2 == 0

# Using the filter function with the named function
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = filter(is_even, numbers)

# Converting the filter object to a list to see the results
even_numbers_list = list(even_numbers)
print(even_numbers_list)  # Output: [2, 4, 6, 8, 10]

```

In both cases, we achieve the same result of filtering out only the even numbers from the list `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`. However, the first example uses the `filter()` function with a lambda function, providing a more concise approach. The second example defines a default (named) function `is_even` to check if a number is even, offering a more structured and readable solution.

## List comprehensions

List comprehensions provide a concise way to create lists in Python by applying an expression to each element in an iterable. They offer a more readable and compact alternative to using loops when building lists. The syntax of a list comprehension consists of square brackets containing an expression followed by a `for` clause, optionally followed by additional `for` or `if` clauses.

**Syntax:**

```python
[expression for item in iterable]

```

**Example 1:**
Creating a list of squares of numbers using a list comprehension:

```python
squares = [x ** 2 for x in range(1, 6)]
print(squares)  # Output: [1, 4, 9, 16, 25]

```

**Example 2:**
Filtering even numbers from a list using a list comprehension:

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [x for x in numbers if x % 2 == 0]
print(even_numbers)  # Output: [2, 4, 6, 8, 10]

```

In these examples:

- The first example creates a list of squares of numbers from 1 to 5 using a list comprehension.
- The second example filters even numbers from a list using a list comprehension with an additional `if` clause.

List comprehensions can also be nested, allowing for more complex operations to be performed. They are widely used in Python for their readability and conciseness, especially when dealing with simple transformations or filtering operations on lists.

- Let's compare list comprehensions with the traditional approach of using loops to achieve similar results.

**Using List Comprehensions:**

```python
# Example 1: Creating a list of squares of numbers
squares = [x ** 2 for x in range(1, 6)]

# Example 2: Filtering even numbers from a list
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [x for x in numbers if x % 2 == 0]

```

**Using Loops:**

```python
# Example 1: Creating a list of squares of numbers with a loop
squares = []
for x in range(1, 6):
    squares.append(x ** 2)

# Example 2: Filtering even numbers from a list with a loop
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = []
for x in numbers:
    if x % 2 == 0:
        even_numbers.append(x)

```

Both approaches achieve the same results, but list comprehensions offer a more concise and readable syntax. They allow you to express the operation in a single line without the need for separate loops and append statements. This can lead to more readable and maintainable code, especially for simple transformations or filtering operations on lists. However, for more complex operations or when you need more control over the iteration process, traditional loops may be more appropriate. It's often a matter of personal preference and the specific requirements of the task at hand.

## zip Function

The `zip()` function in Python is a built-in function that takes iterables (such as lists, tuples, etc.) as input and returns an iterator that produces tuples where the i-th tuple contains the i-th element from each of the input iterables. In other words, it "zips" together the corresponding elements of multiple iterables into tuples.

**Syntax:**

```python
zip(iterable1, iterable2, ...)

```

- `iterable1`, `iterable2`, etc.: The iterables to be zipped together. They can be lists, tuples, or any other iterable object.

**Example:**
Suppose we have two lists representing names and ages, and we want to create a list of tuples where each tuple contains a name and its corresponding age.

```python
names = ["Alice", "Bob", "Charlie"]
ages = [30, 25, 35]

# Using zip to combine the two lists into a list of tuples
combined = list(zip(names, ages))
print(combined)  # Output: [('Alice', 30), ('Bob', 25), ('Charlie', 35)]

```

In this example:

- We have two lists `names` and `ages`.
- We use the `zip()` function to combine these two lists into a list of tuples, where each tuple contains a name from the `names` list and its corresponding age from the `ages` list.
- The `list()` function is used to convert the zip object returned by `zip()` into a list to see the result.

The `zip()` function is commonly used in situations where you need to process multiple iterables together in a pairwise manner. It's useful for tasks like iterating over multiple lists simultaneously or combining data from different sources into a single data structure.

## Stack

In computer science, a stack is a linear data structure that follows the Last-In-First-Out (LIFO) principle, meaning that the most recently added element is the first one to be removed. Think of it like a stack of plates, where you can only add or remove the top plate.

Here are some key characteristics of stacks:

1. **Operations:**
    - **Push:** Adds an element to the top of the stack.
    - **Pop:** Removes the element from the top of the stack.
    - **Peek (or Top):** Returns the element at the top of the stack without removing it.
    - **isEmpty:** Checks if the stack is empty.
    - **Size:** Returns the number of elements in the stack.
2. **Implementation:**
    - Stacks can be implemented using various data structures such as arrays or linked lists.
    - Arrays are commonly used for their simplicity and efficiency in accessing elements.
    - Linked lists can also be used, especially when the size of the stack is dynamic.
3. **Applications:**
    - Stacks are used in many algorithms and programming scenarios, such as:
        - Function call stack in programming languages (for managing function calls and local variables).
        - Undo mechanisms in text editors or software applications.
        - Expression evaluation and parsing (e.g., infix to postfix conversion).
        - Backtracking algorithms.
        - Memory management in operating systems.
        - Browser history navigation.

**Example:**
Let's implement a simple stack using Python's built-in list data structure:

```python
class Stack:
    def __init__(self):
        self.items = []

    def push(self, item):
        self.items.append(item)

    def pop(self):
        if not self.is_empty():
            return self.items.pop()

    def peek(self):
        if not self.is_empty():
            return self.items[-1]

    def is_empty(self):
        return len(self.items) == 0

    def size(self):
        return len(self.items)

# Example usage
stack = Stack()
stack.push(1)
stack.push(2)
stack.push(3)
print("Stack:", stack.items)   # Output: [1, 2, 3]
print("Pop:", stack.pop())     # Output: 3
print("Peek:", stack.peek())   # Output: 2
print("Size:", stack.size())   # Output: 2

```

In this example, we define a `Stack` class with methods for push, pop, peek, isEmpty, and size. We then create an instance of the `Stack` class and perform various stack operations on it.

## Queue

In computer science, a queue is a linear data structure that follows the First-In-First-Out (FIFO) principle, meaning that the first element added to the queue will be the first one to be removed. Think of it like a line at a ticket counter, where the person who arrived first is served first.

Here are some key characteristics of queues:

1. **Operations:**
    - **Enqueue:** Adds an element to the back of the queue.
    - **Dequeue:** Removes the element from the front of the queue.
    - **Peek (or Front):** Returns the element at the front of the queue without removing it.
    - **isEmpty:** Checks if the queue is empty.
    - **Size:** Returns the number of elements in the queue.
2. **Implementation:**
    - Queues can be implemented using various data structures such as arrays or linked lists.
    - Arrays are commonly used for their simplicity and efficiency in accessing elements.
    - Linked lists can also be used, especially when the size of the queue is dynamic.
3. **Applications:**
    - Queues are used in many algorithms and programming scenarios, such as:
        - Job scheduling in operating systems (e.g., CPU scheduling).
        - Network packet handling.
        - Print queue management.
        - Breadth-first search (BFS) traversal in graph algorithms.
        - Task management in multi-threaded environments.

**Example:**
Let's implement a simple queue using Python's built-in list data structure:

```python
class Queue:
    def __init__(self):
        self.items = []

    def enqueue(self, item):
        self.items.append(item)

    def dequeue(self):
        if not self.is_empty():
            return self.items.pop(0)

    def peek(self):
        if not self.is_empty():
            return self.items[0]

    def is_empty(self):
        return len(self.items) == 0

    def size(self):
        return len(self.items)

# Example usage
queue = Queue()
queue.enqueue(1)
queue.enqueue(2)
queue.enqueue(3)
print("Queue:", queue.items)   # Output: [1, 2, 3]
print("Dequeue:", queue.dequeue())   # Output: 1
print("Peek:", queue.peek())   # Output: 2
print("Size:", queue.size())   # Output: 2

```

In this example, we define a `Queue` class with methods for enqueue, dequeue, peek, isEmpty, and size. We then create an instance of the `Queue` class and perform various queue operations on it.

## Tuples

Tuples in Python are ordered collections of elements, similar to lists, but with a few key differences. Here are some important characteristics of tuples:

1. **Immutable:** Tuples are immutable, meaning once they are created, their contents cannot be changed. This means you cannot add, remove, or modify elements in a tuple after it has been created.
2. **Ordered:** Like lists, tuples maintain the order of their elements. You can access elements in a tuple by their index, and the order of elements will remain the same as when the tuple was created.
3. **Heterogeneous:** Tuples can contain elements of different data types. For example, a tuple can contain integers, floats, strings, and other tuples.
4. **Indexed:** Elements in a tuple can be accessed using square brackets and the index of the element, similar to lists. Indexing starts from 0.
5. **Iterable:** Tuples can be iterated over using loops, just like lists and other iterable objects.
6. **Size:** Tuples can contain any number of elements, including zero.

**Syntax:**

```python
my_tuple = (element1, element2, ...)

```

**Example:**

```python
# Creating a tuple
my_tuple = (1, 2, 3, "hello", 3.14)

# Accessing elements
print(my_tuple[0])  # Output: 1
print(my_tuple[-1]) # Output: 3.14

# Iterating over a tuple
for item in my_tuple:
    print(item)

# Tuple unpacking
a, b, c, d, e = my_tuple
print(a, b, c, d, e)  # Output: 1 2 3 hello 3.14

```

Tuples are often used when you want to represent a collection of values that should not be changed throughout the program's execution. They are commonly used for returning multiple values from functions, as keys in dictionaries, or to represent fixed collections of related data.

## Swapping variables

Swapping variables in Python can be easily done using tuple unpacking or by using a temporary variable. Here's how you can do it:

1. **Using Tuple Unpacking:**

```python
a = 5
b = 10

# Swap variables using tuple unpacking
a, b = b, a

print("a:", a)  # Output: 10
print("b:", b)  # Output: 5

```

1. **Using a Temporary Variable:**

```python
a = 5
b = 10

# Swap variables using a temporary variable
temp = a
a = b
b = temp

print("a:", a)  # Output: 10
print("b:", b)  # Output: 5

```

Both methods achieve the same result of swapping the values of variables `a` and `b`. The tuple unpacking method is more concise and Pythonic, while using a temporary variable is more explicit and easier to understand for beginners. Choose the method that best suits your preference and the readability of your code.

## Arrays

In Python, the term "array" can refer to different data structures depending on the context:

1. **List**: Python lists are a dynamic array-like data structure that can hold elements of different data types. Lists are mutable, meaning you can modify their contents after creation. Lists in Python are very flexible and versatile, and they are used extensively in Python programming.
    
    Example:
    
    ```python
    my_list = [1, 2, 3, 4, 5]
    
    ```
    
2. **Array Module**: Python's built-in `array` module provides a more memory-efficient alternative to lists when dealing with arrays of a single data type. Arrays created with the `array` module are typed arrays and more memory efficient compared to lists. However, they are less flexible since they can only store elements of a single data type.
    
    Example:
    
    ```python
    import array
    my_array = array.array('i', [1, 2, 3, 4, 5])
    
    ```
    
3. **NumPy Arrays**: NumPy is a powerful numerical computing library for Python. It provides an array object called `ndarray` which is a multidimensional array of elements of the same type. NumPy arrays are more efficient for numerical operations and are extensively used in scientific computing, data analysis, and machine learning applications.
    
    Example:
    
    ```python
    import numpy as np
    my_numpy_array = np.array([1, 2, 3, 4, 5])
    
    ```
    

Each of these array-like structures has its own advantages and use cases, so the choice depends on the specific requirements of your program. Lists are the most commonly used and most versatile, while `array` module and NumPy arrays offer more specialized functionality and better performance for certain use cases.

## Sets

Suppose we have a list of numbers, and we want to find the unique numbers in that list.

Here's how you can do it with sets:

```python
# Given list of numbers
numbers = [1, 2, 3, 4, 5, 2, 3, 4, 1]

# Convert the list to a set
unique_numbers = set(numbers)

# Print the unique numbers
print("Unique numbers:", unique_numbers)

```

Output:

```
Unique numbers: {1, 2, 3, 4, 5}

```

In this example:

- We start with a list of numbers `numbers`.
- We convert this list to a set using the `set()` function. Since sets only contain unique elements, any duplicates in the list are automatically removed.
- We print out the resulting set of unique numbers.

Sets are handy when you want to remove duplicates from a collection or perform operations that require unique elements. They are easy to use and can help you solve various programming problems efficiently.

## Dictionaries

Dictionaries in Python are unordered collections of key-value pairs. They are used to store and retrieve data in a structured way. Each element in a dictionary is represented as a key-value pair, where the key is used to access its corresponding value. Dictionaries are mutable, meaning you can modify their contents after creation. They are highly versatile and widely used in Python programming.

Here are some key characteristics of dictionaries:

1. **Unordered:** Unlike sequences such as lists, dictionaries do not maintain any order for their elements. The order in which key-value pairs are stored is not guaranteed and may vary.
2. **Mutable:** Dictionaries can be modified after creation. You can add, remove, or update key-value pairs as needed.
3. **Keys:** Keys in a dictionary must be unique and immutable. This means that you cannot have duplicate keys, and keys cannot be lists or dictionaries themselves. Common examples of valid keys are strings, numbers, and tuples.
4. **Values:** Values in a dictionary can be of any data type, including lists, dictionaries, tuples, strings, integers, floats, and more.
5. **Accessing Elements:** Elements in a dictionary are accessed by their keys rather than their index. If you try to access a key that does not exist in the dictionary, a KeyError will be raised.
6. **Dictionary Methods:** Python provides several built-in methods to work with dictionaries, such as `keys()`, `values()`, `items()`, `get()`, `update()`, `pop()`, `popitem()`, and more.

**Syntax:**

```python
my_dict = {key1: value1, key2: value2, ...}

```

**Example:**

```python
# Creating a dictionary
my_dict = {"name": "John", "age": 30, "city": "New York"}

# Accessing elements
print("Name:", my_dict["name"])  # Output: John
print("Age:", my_dict["age"])    # Output: 30

# Adding a new key-value pair
my_dict["gender"] = "Male"
print("Gender:", my_dict["gender"])  # Output: Male

# Removing a key-value pair
del my_dict["city"]
print("Dictionary after removing city:", my_dict)  # Output: {'name': 'John', 'age': 30, 'gender': 'Male'}

```

Dictionaries are commonly used for representing structured data, such as user information, configuration settings, and more. They provide a convenient and efficient way to store and retrieve data in Python.

## Dictionary comprehensions

Dictionary comprehensions in Python provide a concise and efficient way to create dictionaries using an expression and an optional filtering condition. They follow a similar syntax to list comprehensions but produce dictionaries instead.

The syntax for dictionary comprehensions is as follows:

```python
{key_expression: value_expression for item in iterable if condition}

```

Here's a breakdown of each component:

- `key_expression`: Expression to compute keys for the dictionary.
- `value_expression`: Expression to compute values for the dictionary.
- `item`: Variable representing each element in the iterable.
- `iterable`: Iterable object (e.g., list, tuple, set, or any iterable).
- `condition` (optional): Filtering condition to include only certain items in the dictionary (similar to the `if` statement in list comprehensions).

Let's see a simple example to create a dictionary using dictionary comprehension:

```python
# Creating a dictionary of squares using dictionary comprehension
squares = {x: x*x for x in range(1, 6)}

print(squares)

```

Output:

```
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

```

In this example, the dictionary comprehension `{x: x*x for x in range(1, 6)}` creates a dictionary where each key is a number from 1 to 5, and each value is the square of the corresponding key.

You can also add conditions to filter items in the iterable. For example, let's create a dictionary of even squares:

```python
# Creating a dictionary of even squares using dictionary comprehension with condition
even_squares = {x: x*x for x in range(1, 11) if x % 2 == 0}

print(even_squares)

```

Output:

```
{2: 4, 4: 16, 6: 36, 8: 64, 10: 100}

```

In this example, the dictionary comprehension `{x: x*x for x in range(1, 11) if x % 2 == 0}` creates a dictionary where each key is an even number from 1 to 10, and each value is the square of the corresponding key.

Dictionary comprehensions are powerful and provide a concise way to create dictionaries from iterables, especially when combined with conditional expressions for filtering. They are commonly used in Python for creating dictionaries in a more readable and efficient manner.

## Generator

It seems you might be referring to generator expressions in Python. Generator expressions are similar to list comprehensions but instead of creating a list, they create a generator object. Generator expressions are more memory efficient compared to list comprehensions because they generate values on-the-fly rather than storing them in memory all at once.

The syntax for generator expressions is similar to that of list comprehensions, but instead of square brackets (`[]`), you use parentheses (`()`).

Here's the general syntax:

```python
(generator_expression for item in iterable)

```

Let's see an example to illustrate generator expressions:

```python
# Creating a generator expression for generating squares of numbers
squares_generator = (x*x for x in range(1, 6))

# Printing the generator object
print(squares_generator)  # Output: <generator object <genexpr> at 0x7f9b127953c0>

# Iterating over the generator object to get the values
for square in squares_generator:
    print(square)

```

Output:

```
1
4
9
16
25

```

In this example:

- We create a generator expression `(x*x for x in range(1, 6))` to generate the squares of numbers from 1 to 5.
- This generator expression does not produce the actual values immediately. Instead, it generates the values on-the-fly as needed.
- We assign the generator expression to the variable `squares_generator`.
- When we print `squares_generator`, we see that it is a generator object.
- We then iterate over the generator object using a for loop to get the squares of numbers and print them.

Generator expressions are handy when you need to iterate over large sequences of data without storing the entire sequence in memory. They are especially useful for processing large datasets or infinite sequences, as they can be more memory-efficient compared to list comprehensions.

## Unpacking operator

The unpacking operator in Python, denoted by the asterisk (`*`), is a powerful feature that allows you to unpack iterables (such as lists, tuples, or strings) into individual elements. It can be used in various contexts to simplify code and make it more concise.

There are two main use cases for the unpacking operator:

1. **Unpacking into Function Arguments:**
You can use the unpacking operator to pass elements of an iterable as individual arguments to a function. This is particularly useful when the number of arguments is not known beforehand or when you want to apply a function to the elements of a sequence.
    
    ```python
    def add(a, b, c):
        return a + b + c
    
    my_list = [1, 2, 3]
    
    result = add(*my_list)
    print(result)  # Output: 6
    
    ```
    
2. **Unpacking into Iterable:**
You can also use the unpacking operator to unpack elements from one iterable and pack them into another iterable.
    
    ```python
    first_list = [1, 2, 3]
    second_list = [4, 5, 6]
    
    combined_list = [*first_list, *second_list]
    print(combined_list)  # Output: [1, 2, 3, 4, 5, 6]
    
    ```
    
    This can also be used to concatenate multiple iterables together.
    

The unpacking operator can be used with any iterable, including lists, tuples, strings, and sets. It provides a concise and expressive way to work with sequences of elements in Python.
