## DataTypes

__Fundamental Data Types__

int  
float  
bool  
str  
list  
tuple  
set  
dict  

__Classes -> custom types__

__Specialized Data Types__

None

## Python program to find pip version

```python
from importlib import metadata

print("Pip Version : ",metadata.version("pip"))
pip_metadata = metadata.metadata("pip")
print(list(pip_metadata))
print("Homepage: ",pip_metadata["Home-page"])
print("Python requirements",pip_metadata["Requires-Python"])
```

## Python code to check data type and math

```python
print(type(2 + 4))
print(type(2 - 4))
print(type(2 * 4))
print(type(2 / 4))
print(type(10.56))
print(2 ** 3) # 2 power of 3
print(2 // 4) # double division
print(5 // 4) # double division
print(6 % 4) # Modulo
```

## Math functions

```python
#math functions
print(round(3.1))
```

|Function|Description|
|---|---|
|`ceil(x)`        |`Returns the smallest integer greater than or equal to x.`|
|`copysign(x, y)` |`Returns x with the sign of y`|
|`fabs(x)`	       |`Returnsthe absolute value of x`|
|`factorial(x)`   |`Returns the factorial of x`|
|`floor(x)`	   |`Returns the largest integer less than or equal to x`|
|`fmod(x, y)`	   |`Returns the remainder when x is divided by y`|
|`frexp(x)`	   |`Returns the mantissa and exponent of x as the pair (m, e)`|
|`fsum(iterable)` |`Returns an accurate floating point sum of values in the iterable`|
|`isfinite(x)`	   |`Returns True if x is neither an infinity nor a NaN (Not a Number)`|
|`isinf(x)`   |`Returns True if x is a positive or negative infinity`|
|`isnan(x)`	   |`Returns True if x is a NaN`|
|`ldexp(x, i)`	   |`Returns x * (2**i)`|
|`modf(x)`	       |`Returns the fractional and integer parts of x`|
|`trunc(x)`	   |`Returns the truncated integer value of x`|
|`exp(x)`	       |`Returns e**x`|
|`expm1(x)`	   |`Returns e**x - 1`|
|`log(x[, b])`	   |`Returns the logarithm of x to the base b (defaults to e)`|
|`log1p(x)`	   |`Returns the natural logarithm of 1+x`|
|`log2(x)`	       |`Returns the base-2 logarithm of x`|
|`log10(x)`	   |`Returns the base-10 logarithm of x`|
|`pow(x, y)`	   |`Returns x raised to the power y`|
|`sqrt(x)`	       |`Returns the square root of x`|
|`acos(x)`	       |`Returns the arc cosine of x`|
|`asin(x)`	       |`Returns the arc sine of x`|
|`atan(x)`	       |`Returns the arc tangent of x`|
|`atan2(y, x)`	   |`Returns atan(y / x)`|
|`cos(x)`	       |`Returns the cosine of x`|
|`hypot(x, y)`	   |`Returns the Euclidean norm, sqrt(x*x + y*y)`|
|`sin(x)`	       |`Returns the sine of x`|
|`tan(x)`	       |`Returns the tangent of x`|
|`degrees(x)`	   |`Converts angle x from radians to degrees`|
|`radians(x)`	   |`Converts angle x from degrees to radians`|
|`acosh(x)`	   |`Returns the inverse hyperbolic cosine of x`|
|`asinh(x)`	   |`Returns the inverse hyperbolic sine of x`|
|`atanh(x)`	   |`Returns the inverse hyperbolic tangent of x`|
|`cosh(x)`	       |`Returns the hyperbolic cosine of x`|
|`sinh(x)`	       |`Returns the hyperbolic cosine of x`|
|`tanh(x)`	       |`Returns the hyperbolic tangent of x`|
|`erf(x)`	       |`Returns the error function at x`|
|`erfc(x)`	       |`Returns the complementary error function at x`|
|`gamma(x)`	   |`Returns the Gamma function at x`|
|`lgamma(x)`	   |`Returns the natural logarithm of the absolute value of the Gamma function at x`|
|`pi`	           |`Mathematical constant, the ratio of circumference of a circle to it's diameter (3.14159...)`|
|`e`           |`mathematical constant e (2.71828...)`|

## Operator Precedence

```python
# Operator Precedence

print(20 - 3 * 4) #8

print((20 - 3) + 2 ** 2) #21

#()
# **
# * /
# + -
```

## bin()

```python
#bin

print(bin(5))
print(int('0b101', 2))


# Python3 program for implementation
# of int() function
num = 13
 
String = '187'
 
# Stores the result value of
# binary "187" and num addition
result_1 = int(String) + num
print("int('187') + 13 = ", result_1, "\n")
 
# Example_2
str = '100'
 
print("int('100') with base 2 = ", int(str, 2))
print("int('100') with base 4 = ", int(str, 4))
print("int('100') with base 8 = ", int(str, 8))
print("int('100') with base 16 = ", int(str, 16))

#Convert binary string to Python int base
# "111" taken as the binary string
binaryString = "111"
 
# Stores the equivalent decimal
# value of binary "111"
Decimal = int(binaryString, 2)
 
print("Decimal equivalent of binary 111 is", Decimal)
 
# "101" taken as the octal string
octalString = "101"
 
# Stores the equivalent decimal
# value of binary "101"
Octal = int(octalString, 8)
 
print("Decimal equivalent of octal 101 is", Octal)
```

## python keywords

|Keyword|Description|
|---|---|
|`and`	       |`A logical operator`|
|`as`	       |`To create an alias`|
|`assert`	   |`For debugging`|
|`break`	   |`To break out of a loop`|
|`class`	   |`To define a class`|
|`continue`	|`To continue to the next iteration of a loop`|
|`def`	        |`To define a function`|
|`del`	        |`To delete an object`|
|`elif`	    |`Used in conditional statements, same as else if`|
|`else`	    |`Used in conditional statements`|
|`except`	    |`Used with exceptions, what to do when an exception occurs`|
|`False`	    |`Boolean value, result of comparison operations`|
|`finally`	    |`Used with exceptions, a block of code that will be executed no matter if there is an exception or not`|
|`for`	        |`To create a for loop`|
|`from`	    |`To import specific parts of a module`|
|`global`	    |`To declare a global variable`|
|`if`	        |`To make a conditional statement`|
|`import`	    |`To import a module`|
|`in`	        |`To check if a value is present in a list, tuple, etc.`|
|`is`	        |`To test if two variables are equal`|
|`lambda`	    |`To create an anonymous function`|
|`None`	    |`Represents a null value`|
|`nonlocal`	|`To declare a non-local variable`|
|`not`	        |`A logical operator`|
|`or`	        |`A logical operator`|
|`pass`	    |`A null statement, a statement that will do nothing`|
|`raise`	    |`To raise an exception`|
|`return`	    |`To exit a function and return a value`|
|`True`	    |`Boolean value, result of comparison operations`|
|`try`	        |`To make a try...except statement`|
|`while`	    |`To create a while loop`|
|`with`	    |`Used to simplify exception handling`|
|`yield`	    |`To end a function, returns a generator`|

## Variables

```python
a,b,c=1,2,3
print(a)
print(b)
print(c)
```

## Augmented Assignment Operator

```python
some_value = 5
some_value += 2
print(some_value)

some_values = 5
some_values = some_values * 2
print(some_values)
```

## Strings

```python
print(type("Hi Hello there 24!"))
username = 'supercoder'
password = 'supersecret'
long_string = '''
WOW
0 0
---
'''
print(long_string)

first_name = 'Andrei'
last_name = 'Neagoie'
full_name = first_name + ' ' + last_name
print(full_name)
```

## String Concatenation

```python
# string concatenation
print('hello'+' Andrei')
```

## Type Concatenation

```python
print(type(str(100)))
print(type(int((str(101)))))
a = str(100)
b = int(a)
c = type(b)
print(c)
```

## Escape Sequence

```python
print(type(str(100)))
print(type(int((str(101)))))
a = str(100)
b = int(a)
c = type(b)
print(c)
```

## Formatted strings

```python
# formated strings

name = 'Johnny'
age = 55

print(f'hi {name}, you are {age} years old')

print('hi {}, you are {} years old'.format(name,age))

print('hi {new_name}, you are {age} years old'.format(new_name='sally',age=100))
```

## string indexes

```python
selfish = 'me me me'
        #  01234567
print(selfish[7])
print(selfish)
# [start:stop]
print(selfish[0:2])
# [start:stop:stepover]
print(selfish[0:8:2])
# [start:]
print(selfish[1:])
# [:end]
print(selfish[:5])
# [::end]
print(selfish[::1])
# [-1] This will do reverse
print(selfish[-1])
# [::-1] Reverse an order or string
print(selfish[::-1])
```

## Immutability

```python
selfish = '01234567'

#selfish = 100
#print(selfish)

selfish = selfish + '8' # This will replace whole selfish data
print(selfish)

selfish[0] = '8'
#here there will be error, because strings are immutable
```

```
There are mutable and Immutable types of Pythons built in types Mutable built-in types 
 
List 
Sets 
Dictionaries 
Immutable built-in types 
 
Strings 
Tuples 
Numbers 
```

## Bultin Functions + Methods

```python
## Built-in Functions + Methods

# Refer to python built functions url: https://docs.python.org/3/library/functions.html
# Refer to string methods url: https://www.w3schools.com/python/python_ref_string.asp
print(len('hellloooo'))

greet = 'hellloooo'
print(greet[0:len(greet)])


quote = 'to be or not to be'
print(quote.upper())

print(quote.capitalize())

print(quote.lower())

print(quote.find('be'))

print(quote.replace('be','me'))

print(quote)

quote2 = quote.replace('be','me')
print(quote2)
print(quote)
```

## Booleans

```python
#booleans

name = 'Andrei'
is_cool = False

is_cool = True

print(bool(1))
print(bool(0))

print(bool('True'))
```

## Exercise: Type Conversion

```python
## Exercise: Type Conversion

name = 'Andrei Neagoie'
ages = 50
relationship_status = 'single'

relationship_status = 'it\'s complicated'

print(relationship_status)

birth_year = input('What year were you born?')
print(type(birth_year))

age = 2019 - float(birth_year)
print(f'You are {age} years old')
```

# Developer Fundamentals II

```python
#python commenting practices url :https://realpython.com/python-comments-guide/

fundnamae = 'Andrei'
is_cool = False
is_cool = True

"""
This is quite a long comment
It is a multiline comment
"""

print(bool('True'))
```

## Exercise: Password Checker

```python
## Exercise: Password Checker
# input('jayjay')
# input('secret')
# print('{username}, your password {*****} is {6} letters long')
# print('*' * 10)

username=input('What is your username?')
password=input('What is your password?')

password_length = len(password)
hidden_password = ('*' * password_length)

print(f'{username}, your password {hidden_password} is {len(password)} letters long')
```

## Lists

```python
## lists

#li = [1,2,3,4,5]
#li2 = ['a','b','c']
#li3 = [1,2,'a',True]

amazon_cart = ['notebooks', 'sunglasses', 'toys', 'books', 'guitar']
print(amazon_cart[1])
```

## list slicing

```python
#list slicing
#string = 'helllooo'
#string[0:2:1]
# Exmaple: https://replit.com/@aneagoie/lists#main.py
amazon_cart = ['notebooks', 'sunglasses', 'toys', 'grapes']
# print(amazon_cart[0:2])

amazon_cart[0] = 'laptop'
# new_cart = amazon_cart[0:3]
new_cart = amazon_cart[:]
new_cart[0] = 'gum'
print(new_cart)
print(amazon_cart)
```

## Matrix

```python
## Matrix

matrix = [
    [1, 2, 3], 
    [4, 5, 6], 
    [7, 8, 9]
    ]

print(matrix[0][1])
```

## List methods

```python
## List method

# list method url : https://www.w3schools.com/python/python_ref_list.asp

basket = [1,2,3,4,5]
#print(len(basket))

# append
basket.append(100)
new_list = basket
new_lists = basket.append(101)
print(basket)
print(new_list)
print(new_lists)

basket.insert(4,104)
news = basket
print(news)

basket.extend([106])
new_lists5 = basket
print(new_lists5)

# pop

basket.pop()
basket.pop(0)
print(basket)

# remove

basket.remove(4)
print(basket)

# clear

basket.clear()
new_lists7 = basket
print(new_lists7)
```

## List methods 2

```python
## List methods 2

# list method 2 url https://www.w3schools.com/python/python_ref_keywords.asp
# relpit url: https://replit.com/@aneagoie/lists-2

basket = ['a', 'b', 'c', 'd', 'e','d']
print(basket.index('d',0,4))

print('x' in basket)
print('i' in 'hi my name is Ian')

print(basket.count('d'))
```

## List methods 3

```python
## list methods 3

basket = ['a', 'b', 'c', 'd', 'e','d']
basket.sort()
print(basket)
new_basket = ['x','a', 'b', 'c', 'd', 'e','d']
print(sorted(new_basket))

new_basket1 = new_basket[:]
new_basket1.sort()
print(new_basket1)

new_basket2 = new_basket.copy()
new_basket2.sort()
print(new_basket2)

new_basket.reverse()
print(new_basket)
```

## Command List Patterns

```python
# Excercise https://replit.com/@aneagoie/lists-3

basket = ['x','a', 'b', 'c', 'd', 'e','d']
basket.sort()
basket.reverse()
print(basket)
#print(basket[::-1])
#print(basket[:])
#print(basket)
#print(list(range(1,100))) 1 to 99
#print(list(range(100))) # 0 t0 99

sentence = ''
new_sentence = sentence.join(['hi','my','name','is','JOJO'])
print(new_sentence)
```

## List unpacking

```python
## List unpacking
#a,b,c = [1,2,3]
a,b,c, *other,d = [1,2,3,4,5,6,7,8,9]
print(a)
print(b)
print(c)
print(other)
print(d)
```

## None

```python
weapons = None
print(weapons)
```
## Dictionaries

```python
## Dictionary
dictionary = {
    'a':1,
    'b':2,
    'x':3
}

print(dictionary['b'])
print(dictionary)

dictionary1 = {
    'a':[1,2,3],
    'b':'hello',
    'x':True
}

print(dictionary1)
print(dictionary1['a'][1])

my_list = [
    {
        'a': [1,2,3],
        'b': 'hello',
        'x': True
    },
    {
        'a': [4,5,6],
        'b': 'hello',
        'x': True
    }
]
print(my_list[0]['a'][2])
```

# Developer Fundamentals III

```python
## Developer Fundamentals III

dictionary = {
    'weapons': [1,2,3],
    'greeting': 'hello',
    'is_Magic': True
}

print(dictionary['weapons'][1])
```

## Dictionary Keys

```python
## Dictionary Keys

dictionary = {
    123: [1,2,3],
    'greeting': 'hello',
    'is_Magic': True
}
print(dictionary[123])

dictionary1 = {
    123: [1,2,3],
    123: 'hello'
}

print(dictionary1[123])
```

## Dictionary Methods

```python
## Dictionary Methods
##referemce url: https://www.w3schools.com/python/python_ref_dictionary.asp

users = {
    'basket': [1,2,3],
    'greet': 'hello',
    'age': 20
}
print(users.get('age', 55)) # If age does not exists it will override with 55

users2 = dict(name='JohnJohn')
print(users2)
```

## Dictionary Methods 2

```python
## Dictionary Methods 2
## url https://replit.com/@aneagoie/dictionary

user = {
    'basket': [1,2,3],
    'greet': 'hello',
    'age': 20
}
print('basket' in user)
print('size' in user)
print('hello' in user.values())
print('hello' in user.items())
print(user.items())
user2 = user.copy()
user3 = user.copy()
user.clear()
print(user)
print(user2)

user2.pop('age')
print(user2)

print(user2.popitem())
print(user2)

print(user2.update({'age': 55}))
print(user2)
```

## Tuples

```python
# Tuple
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[1])
print(5 in my_tuple)

user = {
    (1,2): [1,2,3],
    'greet': 'hello',
    'age': 20
}

print(user[(1,2)])
```

## Tuples 2

```python
## Tuples 2
# https://www.w3schools.com/python/python_ref_tuple.asp

my_tuple = (1, 2, 3, 4, 5, 5)
mew_tuple = my_tuple[1:2]
print(mew_tuple)

x,y,z, *other = (1, 2, 3, 4, 5)
print(x,y,z,other)

print(my_tuple.count(5))
print(my_tuple.index(5))
print(len(my_tuple))
```

## Sets

```python
## Sets
my_set = {1, 2, 3, 4, 5, 5}
my_set.add(100)
my_set.add(2)
print(my_set)

my_list = [1,2,3,4,5,5]
print(set(my_list))
print( 1 in my_set)
print(len(my_set))
print(list(my_set))

new_set = my_set.copy()
my_set.clear()
print(my_set)
print(new_set)
```

## Sets2

```python
my_set = {1,2,3,4,5,5}
your_set = {4, 5, 6, 7, 8, 9, 10}

# https://www.w3schools.com/python/python_ref_set.asp
# https://replit.com/@aneagoie/sets

# print(my_set.difference(your_set))
# print(my_set)
# print(my_set.discard(5))
# print(my_set)
# print(my_set.difference_update(your_set))
# print(my_set)
# print(my_set & your_set)
# print(my_set.intersection(your_set))
# print(my_set.isdisjoint(your_set))
# print(my_set.union(your_set))
# print(my_set | your_set)

my_sets = {4,5}
your_sets = {4, 5, 6, 7, 8, 9, 10}

print(my_sets.issubset(your_sets))
print(your_sets.issuperset(my_sets))
```

## conditional Logic

```python
is_old = True
is_licensed = True

if is_old and is_licensed:
  print("You are old enough to drive, with license!")
else:
  print("You cannot drive")
```

__Reference:__ https://stackoverflow.com/questions/39983695/what-is-truthy-and-falsy-how-is-it-different-from-true-and-false

## Ternary Opeartor

```python
# Ternary Operator

# condition_if_true if condition else condition_if_false

is_friend = True
can_message = "Message allowed" if is_friend else "Not allowed"
print(can_message)
```

## Short circuiting

```python
# short circuiting

is_Friend = False
is_User = True

if is_Friend and is_User:
    print('best friends forever')
else:
    print('just friends')

if is_Friend or is_User:
    print('best friends forever')
else:
    print('just friends')
```

## Logical Operators

```python
## Logical Operator

print('a' > 'A') # True

print(1 < 2 > 3 < 4) # False

print(0 != 0)

# < > == >= <= !=
# and or not 
```

## Exercise: Logical Operators

```python
is_magician = True
is_expert = False

if is_expert and is_magician:
    print("You are a master magician!")
elif is_magician and not is_expert:
    print("At least you're getting there")
elif not is_magician:
    print("You need magic powers")
```

## is vs ==

```python
## is vs ==

print(True ==  1)
print('' == 1)
print([] == 1)
print(10 == 10.0)
print([] == [])

print('=========')
print(True ==  1)
print('1' == 1)
print([] == 1)
print(10 == 10.0)
print([1,2,3] == [1,2,3])

print('=========')
print(True is 1)
print('1' is 1)
print([] is 1)
print(10 is 10.0)
print([1,2,3] is [1,2,3])

print('=========')
print(True is True)
print('1' is '1')
print([] is 1)
print(10 is 10)
a = [1,2,3]
b = a
c = [1,2,3]
print(a is b)
print(a is c)
```

## For Loops

```python
for item in 'Zero to Mastery':
    print(item)

for item in {1,2,3,4,5}:
    print(item)

for item in [1,2,3,4,5]:
    print(item)

for item in (1,2,3,4,5):
    print(item)

for item in (1,2, 3, 4, 5):
    for x in ['a','b', 'c']:
        print(item, x)
```

## Iterables

```python
user = {
    'name': 'Golem',
    'age': 7,
    'can_swim': False
}

for item in user.items():
    print(item)

for item in user.values():
    print(item)

for item in user.keys():
    print(item)

for x,y in user.items():
    print(x,':',y)

for item in user.items():
    key,value = item;
    print(key,'=',value)

#iterable - list, dictionary, tuple, set, string
#iterate -> one by one check each item in the collection
```
## Excercise Tricky counter

```python
# counter
my_list = [1,2,3,4,5,6,7,8,9,10]

counter = 0
for item in my_list:
    counter += item
    print(counter)


print("Outside for loop: ", counter)
```

## Range

```python
for number in range(1, 100):
    print(number)

print('================')

for _ in range(0, 10, 2):
    print(_)

print('================')

for _ in range(0, 10, -1):
    print(_)

print('================')

for _ in range(10, 0):
    print(_)

print('================')

for _ in range(10, 0, -1):
    print(_)

print('================')

for _ in range(2):
    print(list(range(10)))
```

## Enumerate

```python
for i,char in enumerate('Hellloooo'):
    print(i,char)

print('=========')

for i,char in enumerate([1,2,3]):
    print(i,char)

print('=========')

for i,char in enumerate(list(range(100))):
    print(i,char)

print('=========')

for i,char in enumerate(list(range(100))):
    print(i,char)
    if char == 50:
        print(f'index of 50 is {i}')
```
## While Loops

```python
i = 0
while i < 50:
    print(i)
    break
print('====================')
i = 0
while i < 50:
    print(i)
    i = i + 1
print('====================')
i = 0
while i < 50:
    print(i)
    i += 1
print('====================')
i = 0
while i < 50:
    print(i)
    i += 1
else:
    print('i is over 50')
print('====================')
i = 0
while i < 50:
    print(i)
    i += 1
    break
else:
    print('i is over 50')
```

## While Loops 2

```python
for item in [1,2,3]:
    print(item)

print('====================')

i = 0
while i < len([1,2,3]):
    print(i)
    i += 1

print('====================')

my_list = [1,2,3]
for item in my_list:
    print(item)

print('====================')

i = 0
while i < len(my_list):
    print(my_list[i])
    i += 1

print('====================')

while True:
    input('say something: ')
    break

print('====================')

while True:
    response = input('say something: ')
    if (response == 'bye'):
        break
```

## break, continue, pass

```python
my_list = [1,2,3]
for item in my_list:
    print(item)
    break

i = 0
while i < len(my_list):
    print(my_list[i])
    i += 1
    break

print('====================')

my_list = [1,2,3]
for item in my_list:
    continue
    print(item)

i = 0
while i < len(my_list):
    i += 1
    continue
    print(my_list[i])

print('====================')

my_list = [1,2,3]
for item in my_list:
    pass

i = 0
while i < len(my_list):
    print(my_list[i])
    i += 1
    pass

print('====================')
```

## Our First GUI

```python
#Exercise!
#Display the image below to the right hand side where the 0 is going to be ' ', and the 1 is going to be '*'. This will reveal an image!
picture = [
  [0,0,0,1,0,0,0],
  [0,0,1,1,1,0,0],
  [0,1,1,1,1,1,0],
  [1,1,1,1,1,1,1],
  [0,0,0,1,0,0,0],
  [0,0,0,1,0,0,0]
]

for row in picture:
    for pixel in row:
        if (pixel == 1):
            print('*', end='')
        else:
            print(' ', end='')
    print('')
```

# DEVELOPER FUNDAMENTALS : IV

## Find Duplicates

```python
# Exercise: check for duplicates in list:

some_list = ['a', 'b', 'c', 'b', 'd', 'm', 'n', 'n']

## duplicates = set([x for x in some_list if some_list.count(x) > 1])

duplicates = []

for value in some_list:
    if some_list.count(value) > 1:
        if value not in duplicates:
            duplicates.append(value)

print(duplicates)

singleduplicates = []
singleduplicates = [ values for values in some_list if some_list.count(values) > 1 if values in singleduplicates]
```
