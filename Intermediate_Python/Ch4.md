# Intermediate Python for Data Science

## Chapter 4 - Loops

### while: warming up

recipe

```python

while condition :
    expression

```

### Basic while loop


```python

# Initialize offset
offset = 8

# Code the while loop
while offset != 0:
    print("correcting...")
    offset = offset - 1
    print(offset)

```


### Add conditionals

```python


# Initialize offset
offset = -6

# Code the while loop
while offset != 0 :
    print("correcting...")
    if offset > 0 :
        offset = offset -1 

    else : 
        offset = offset +1
    print(offset)

```


