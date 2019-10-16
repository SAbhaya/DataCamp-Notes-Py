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





