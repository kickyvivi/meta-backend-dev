# Notes for Week 1

## Welcome to Python Programming

### Python syntax cheat sheet
- Newline:
```python
x = 1 + 2 \
    + 3
```
Here even though 3 is written in 2nd line, there is no error. Explicitly specified newline using '\\'
- Indentation:
    - `def say_hello(): print("Hello there!")`

### Variables
- camelCase
- snake_case
- Simple assignment : `a = 10`
- Multiple variables same value : `a=b=c=10`
- Multiple assignment : `a,b,c = 10,20,30`
- Deleting a variable : `del a`

### Basic Data types
- A data type is an attribute associated with a piece of data that tells a computer system how to interpret its value
- 5 types of literals:
    - Numeric
    - Sequence
    - Boolean
    - Dictionary
    - Set
- ![Data types in Python](./Data%20types.png)
- Finc type of data : `type()`
```python
>>> a = 10+10j
>>> a
(10+10j)
>>> type(a)
<class 'complex'>
```
- Examples:
```python
a = 10
b = 2.3
c = 10 + 20j
d = 'abc'
e = [1,2,'a',4.4]
f = (1,2,3,4,'abc')
g = {'a':1, 'b':2}
h = True
i = {1,2,3,'abc'}

print(type(a))
print(type(b))
print(type(c))
print(type(d))
print(type(e))
print(type(f))
print(type(g))
print(type(h))
print(type(i))
```
```python
<class 'int'>
<class 'float'>
<class 'complex'>
<class 'str'>
<class 'list'>
<class 'tuple'>
<class 'dict'>
<class 'bool'>
<class 'set'>
```

### Strings
- Single line: `"This is a single line of string"`
- Multi-line:
```python
print("This is too \
big to fit in \
a single line")
```
```
This is too big to fit in a single line
```
```python
a = 'This is too ' \
    'big to fit in '\
    'a single line.'
print(a)
```
```
This is too big to fit in a single line.
```

### Basic Data type and Function Cheatsheet
```python
print(int(10.9))
print(float(10))
print(str(55))
print(len('This function will print the length of this string'))
print(ord('a')) #print the Unicode (ASCII) value
```
```
10
10.0
55
50
97
```
### input()
```python
print("Where do you live?")
location = input()
print("So you live in " + location)
```
```
So you live in India
```

### Type casting
- Implicit
    - Automatic
    - For compatible data types
    - Type Error (E.g.: Str > Int)
- Explicit
```python
print(ord('a'))
print(hex(12))
print(oct(121))
print(tuple('a'))
print(set('a'))
print(list('a'))
print(dict([('a',1),('b',2)]))
```
```
97
0xc
0o171
('a',)
{'a'}
['a']
{'a': 1, 'b': 2}
```

### User input, console output
- input()
    - Returns string
- print()
- Arguments for print():
    1. object
    2. sep
    3. end
    4. file
    5. flush
- .format() in print()

E.g. 1
```python
str1 = input("Enter first name: ")
str2 = input("Enter last name: ")
print('Hello {0} {1}'.format(str1, str2))
```
```
Enter first name: Tom
Enter last name: Jone
Hello Tom Jone
```
E.g. 2
```python
str1 = input("Enter first name: ")
str2 = input("Enter last name: ")
print('Hello {1} {0}'.format(str1, str2))
```
```
Enter first name: Tom
Enter last name: Jone
Hello Jone Tom
```
E.g. 3
```python
str1 = input("Enter first name: ")
str2 = input("Enter last name: ")
print('Hello {} {}'.format(str1, str2))
```
```
Enter first name: Tom
Enter last name: Jone
Hello Tom Jone
```
