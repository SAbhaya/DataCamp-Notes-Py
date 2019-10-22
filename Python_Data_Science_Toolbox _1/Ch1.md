# Python Data Science Toolbox (Part 1)

## Chapter 1 - Writing your own functions

### Strings in Python

+ operator concatenates strings 
* concatenates multiple copies of a string together

### Recapping built-in functions

y1: y1 = str(x)
y2: y2 = print(x)
Check the types of the variables x, y1, and y2

```python

In [4]: type(y1)
Out[4]: str

In [5]: type(y2)
Out[5]: NoneType

In [6]: type(x)
Out[6]: float

```

### Write a simple function

```python

# Define the function shout
def shout():
    """Print a string with three exclamation marks"""
    # Concatenate the strings: shout_word
    shout_word = 'congratulations' + '!'*3

    # Print shout_word
    print(shout_word)

# Call shout
shout()

```
### Single-parameter functions

```python

# Define shout with the parameter, word
def shout(word):
    """Print a string with three exclamation marks"""
    # Concatenate the strings: shout_word
    shout_word = word + '!!!'

    # Print shout_word
    print(shout_word)

# Call shout with the string 'congratulations'
shout('congratulations')

```

### Functions that return single values

```python

# Define shout with the parameter, word
def shout(word):
    """Return a string with three exclamation marks"""
    # Concatenate the strings: shout_word
    shout_word = word + '!!!'

    # Replace print with return
    return(shout_word)

# Pass 'congratulations' to shout: yell
yell = shout('congratulations')

# Print yell
print(yell)

```

### Functions with multiple parameters

```python

# Define shout with parameters word1 and word2
def shout(word1, word2):
    """Concatenate strings with three exclamation marks"""
    # Concatenate word1 with '!!!': shout1
    shout1 = word1 + '!!!'
    
    # Concatenate word2 with '!!!': shout2
    shout2 = word2 + '!!!'
    
    # Concatenate shout1 with shout2: new_shout
    new_shout = shout1 + shout2

    # Return new_shout
    return new_shout

# Pass 'congratulations' and 'you' to shout(): yell
yell = shout('congratulations','you')

# Print yell
print(yell)

```

### A brief introduction to tuples

define tuple,

> `tuple1 = (3, 4, 6)`

Unpack tuple

> `a, b, c = tuple1`



```python

# Unpack nums into num1, num2, and num3
num1, num2, num3 = nums

# Construct even_nums
even_nums = (2, num2, num3)

```
### Functions that return multiple values

```python

# Define shout_all with parameters word1 and word2
def shout_all(word1, word2):
    
    # Concatenate word1 with '!!!': shout1
    shout1 = word1 + '!!!'
    
    # Concatenate word2 with '!!!': shout2
    shout2 = word2 + '!!!'
    
    # Construct a tuple with shout1 and shout2: shout_words
    shout_words = (shout1 ,shout2)

    # Return shout_words
    return shout_words

# Pass 'congratulations' and 'you' to shout_all(): yell1, yell2
yell1, yell2 = shout_all('congratulations', 'you')

# Print yell1 and yell2
print(yell1)
print(yell2)

```

### Bringing it all together (1)





