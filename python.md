# Python
[Python Defined Keywords](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


## 1. Comments:
```<Python>
# This is a comment.
```
```<Python>
'''
This is a block comment.
'''
```

## 2. Variables:
```<Python>
x = 5
x, y = 1, 2      # Many Variables, Many Value
a = b = c = 0    # Many Variables, One Value
```
```<Python>
# Unpacking a Collection:
fruits = ["apple", "orange", "mango"]
p, q, r = fruits
```
```<Python>
# Globalize a Localized Variable
def function1():
    x = 10
    global x  # Wrong! first define, then assign! 
```

## 3. Data Types:

### _Text Type:_ (STRING)
```python    
    str
    example: 
        "name" 
```
### _Numeric Types:_ (INTEGER, FLOAT, COMPLEX)
```python
    int | float | complex
    example: 
        86, 86.0 or 8.6e1, 86j
```
### _Sequence Type:_ (LIST, TUPLE, RANGE)
```python
    list | tuple | range
    example: 
        fruitList = ["cherry", "pineapple", "grapes"]
        fruitTuple = ("cherry", "grapes")
        rangeFrom0to5 = range(6)
```    
```python
type(range(6)) 
# <class 'range'> 
```      

### _Mapping Type:_ (DICTIONARY)
```python
    dict
    example:
        myDict = { 'name':'Sam', 'age':22 }
```
### _Set Type:_ (SET, FROZENSET)
```python
    set | frozenset
    example:
        { 4, 5, "number" }
        # This is a set where the sequence is random.
        frozenset( { 4, 5, "number" } )
        # This is a frozenset where the sequence is frozen. 
```
### _Boolean Type:_ (BOOLEAN)
```python
    bool
    example (Only *two* values):
        True
        False
    
    # Note: TRUE, true, FALSE, false are undefined!
```
### _Binary Type:_ (BYTES, BYTEARRAY, MEMORYVIEW)
```python
    bytes, bytearray, memoryview
    example:
        b"hello" or bytes("hello")
        bytearray(b"hello")
        memoryview(b"hello")
    
    # These binary datatypes are essential for doing binary manipulation.
```
### _None Type:_ (NONE)
```python
    NoneType
    example: (Only 1 value)
        None

    # Note: NONE, none are not defined!
    # If assigned to a variable, the variable outputs nothing!
```

## 4. Type Conversion / Type Casting:
```python
int(x)
float(x)
complex(x)
str(x)
```

## 5. Random Number:
```python
import random
random.randrange(1,10)
```

## 6. Python Strings:
```python
    "My name is 'John'!"
    a = '''this,
    is a multiline
    string.'''
```



+ Chaining Rule: Most inner function would run first.
+ type( object )   # Returns object type
+ id( object )     # Returns memory address of the object
+ len( object )    # Returns length of the object

#### methods:
+ object_name.method(*param*)
+ object_name.attr


+ all indexes ...
+ Explore 46 Str methods with one example


<br />

### *The notes below display all the methods related to strings str in python. These notes are created using Prompt Engineering and Generative AI (OpenAI).*

<br />

# String Methods Applied to "hello, world!"

```python
myStr = "hello, world!"
myStr2 = "Name\tAge\tOccupation"
```
1. **Capitalize:**
   - `myStr.capitalize()`
   - Result: `"Hello, world!"`

2. **Casefold:**
   - `myStr.casefold()`
   - Result: `"hello, world!"`

3. **Center:**
   - `myStr.center(20)`
   - Result: `"   hello, world!    "`

4. **Count:**
   - `myStr.count('l')`
   - Result: `3`

5. **Encode:**
   - `myStr.encode()`
   - Result: `b'hello, world!'`

6. **Endswith:**
   - `myStr.endswith('!')`
   - Result: `True`

7. **Expandtabs:**
   - `myStr2.expandtabs(4)`
   - Result: `"Name        Age         Occupation"`

8. **Find:**
   - `myStr.find('world')`
   - Result: `7`

9. **Format:**
   - `myStr.format()`
   - Result: `"hello, world!"` (no placeholders to replace)

10. **Index:**
    - `myStr.index('world')`
    - Result: `7`

11. **Isalnum:**
    - `myStr.isalnum()`
    - Result: `False`

12. **Isalpha:**
    - `myStr.isalpha()`
    - Result: `False`

13. **Isascii:**
    - `myStr.isascii()`
    - Result: `True`

14. **Isdecimal:**
    - `myStr.isdecimal()`
    - Result: `False`

15. **Isdigit:**
    - `myStr.isdigit()`
    - Result: `False`

16. **Isidentifier:**
    - `myStr.isidentifier()`
    - Result: `False`

17. **Islower:**
    - `myStr.islower()`
    - Result: `True`

18. **Isnumeric:**
    - `myStr.isnumeric()`
    - Result: `False`

19. **Isprintable:**
    - `myStr.isprintable()`
    - Result: `True`

20. **Isspace:**
    - `myStr.isspace()`
    - Result: `False`

21. **Istitle:**
    - `myStr.istitle()`
    - Result: `False`

22. **Isupper:**
    - `myStr.isupper()`
    - Result: `False`

23. **Join:**
    - `'-'.join(['hello', 'world'])`
    - Result: `"hello-world"`

24. **Ljust:**
    - `myStr.ljust(20)`
    - Result: `"hello, world!       "`

25. **Lower:**
    - `myStr.lower()`
    - Result: `"hello, world!"`

26. **Lstrip:**
    - `myStr.lstrip()`
    - Result: `"hello, world!"`

27. **Maketrans:**
    - `myStr.maketrans('h', 'H')`
    - Result: `{104: 72}`

28. **Partition:**
    - `myStr.partition(',')`
    - Result: `('hello', ',', ' world!')`

29. **Removeprefix:**
    - `myStr.removeprefix('hello')`
    - Result: `", world!"`

30. **Removesuffix:**
    - `myStr.removesuffix('!')`
    - Result: `"hello, world"`

31. **Replace:**
    - `myStr.replace('world', 'there')`
    - Result: `"hello, there!"`

32. **Rfind:**
    - `myStr.rfind('o')`
    - Result: `8`

33. **Rindex:**
    - `myStr.rindex('o')`
    - Result: `8`

34. **Rjust:**
    - `myStr.rjust(20)`
    - Result: `"       hello, world!"`

35. **Rpartition:**
    - `myStr.rpartition('o')`
    - Result: `('hell', 'o', ', world!')`

36. **Rsplit:**
    - `myStr.rsplit()`
    - Result: `['hello,', 'world!']`

37. **Rstrip:**
    - `myStr.rstrip()`
    - Result: `"hello, world!"`

38. **Split:**
    - `myStr.split()`
    - Result: `['hello,', 'world!']`

39. **Splitlines:**
    - `myStr.splitlines()`
    - Result: `['hello, world!']`

40. **Startswith:**
    - `myStr.startswith('hello')`
    - Result: `True`

41. **Strip:**
    - `myStr.strip()`
    - Result: `"hello, world!"`

42. **Swapcase:**
    - `myStr.swapcase()`
    - Result: `"HELLO, WORLD!"`

43. **Title:**
    - `myStr.title()`
    - Result: `"Hello, World!"`

44. **Translate:**
    - `myStr.translate(myStr.maketrans('h', 'H'))`
    - Result: `"Hello, world!"`

45. **Upper:**
    - `myStr.upper()`
    - Result: `"HELLO, WORLD!"`

46. **Zfill:**
    - `myStr.zfill(20)`
    - Result: `"0000000hello, world!"`
