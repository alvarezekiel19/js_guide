# 🐍 Lightsailor's Python Cheatsheet

# 📦 1. Variables and Data Types
```py
# Numbers
x = 10        # Integer
y = 3.14      # Float

# Strings
name = "Francis"

# Booleans
is_active = True

# Lists
fruits = ["apple", "banana", "cherry"]

# Tuples
coords = (1, 2)

# Dictionaries
person = {"name": "Francis", "age": 25}

# Sets
unique_values = {1, 2, 3}
```

# 🖨️ 2. Printing
```py
print("Hello, World!")
print("Name:", name)
print(f"Name is {name} and age is {person['age']}")
```

# 🧮 3. Comparison Operators
```py
==   # Equal to
!=   # Not equal to
>    # Greater than
<    # Less than
>=   # Greater than or equal to
<=   # Less than or equal to

# Example:
if x >= 10:
    print("x is at least 10")
```

# 🔀 4. Logical Operators
```py
and     # True if both are True
or      # True if at least one is True
not     # Inverts the boolean value

# Example:
if x > 5 and is_valid:
    print("x is valid and greater than 5")

if not is_valid:
    print("Invalid")
```

# 🔎 5. Membership Operators
```py
in      # True if value is in sequence
not in  # True if value is NOT in sequence

# Examples in conditionals:
if "apple" in fruits:
    print("Apple is in the list.")

if "kiwi" not in fruits:
    print("Kiwi is not in the list.")

# Examples in loops:
for fruit in fruits:
    if "a" in fruit:
        print(f"{fruit} contains 'a'")
```

# 🧾 6. Conditionals
### ➤ Standard
```py
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is 5")
else:
    print("x is less than 5")
```

### ➤ One-Line Conditional
```py
expression_if_true if condition else expression_if_false
# Can be used in variables and return statements
```


# 🔁 7. Loops
### 🔁 For loop
```py
for fruit in fruits:
    print(fruit)

for i in range(5):  # 0 to 4
    print(i)
```

### 🔁 While Loop
```py
count = 0
while count < 5:
    print(count)
    count += 1
```

# 🧰 8. Functions
```py
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```

# 🔄 9. Typecasting
```py
int("5")          # 5
float("3.14")     # 3.14
str(100)          # "100"
bool("")          # False
bool("hello")     # True
list("abc")       # ['a', 'b', 'c']
tuple([1, 2])     # (1, 2)
set([1, 2, 2])    # {1, 2}
```

# 🔧 10. Common Built-in Methods
### ✅ String Methods
```py
text = "hello world"

text.upper()         # 'HELLO WORLD'
text.lower()         # 'hello world'
text.capitalize()    # 'Hello world'
text.split()         # ['hello', 'world']

# SPLIT ex.
"Hello".split("l")   # ['He', '', 'o']
"Hellllo".split("l")   # ['He', '', '', 'o']

text.replace("world", "Python")  # 'hello Python'
" ".join(["hello", "world"])     # 'hello world'
"hello123".isalnum()  # True
"hello!".isalnum()    # False
```

### ✅ List Methods
```py
nums = [1, 2, 3]

nums.append(4)
nums.remove(2)
nums.pop()           # Removes last item
nums.sort()
nums.reverse()       # Reverses the list in place
len(nums)
" ".join(["a", "b", "c"])  # 'a b c'  (useful when list items are strings)
```

### ✅ Dictionary Methods
```py
person = {"name": "Bob", "age": 25}

person.get("name")
person.keys()
person.values()
person.items()
```

### ✅ Set Methods
```py
s = {1, 2, 3}

s.add(4)
s.remove(1)
3 in s
```

# 💡 11. Other Useful Built-ins
```py
len("hello")
type(3.14)
sum([1, 2, 3])
max([1, 9, 3])
min([1, 9, 3])
sorted([3, 1, 2])
range(1, 5)
```