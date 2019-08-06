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

### for loop

### loop over a list

```python
# areas list
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Code the for loop
for area in areas:
    print(area)


```


### Indexes and values

Using `for` loop to iterate over a list

`enumerate()` to access the index

```

fam = [1.73, 1.68, 1.71, 1.89]
for index, height in enumerate(fam) :
    print("person " + str(index) + ": " + str(height))

```

```python

# areas list
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Change for loop to use enumerate() and update print()
for index, a in enumerate(areas) :
    print("room " + str(index) +": " + str(a))
    
```

replace index 0 with 1..

```python

# areas list
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Code the for loop
for index, area in enumerate(areas) :
    print("room " + str(index +1) + ": " + str(area))

```

### Loop over list of lists

```python

# house list of lists
house = [["hallway", 11.25], 
         ["kitchen", 18.0], 
         ["living room", 20.0], 
         ["bedroom", 10.75], 
         ["bathroom", 9.50]]
         
# Build a for loop from scratch
for room in house:
    print("the " +room[0]+ " is " + str(room[1]) + " sqm" )

```


### Loop over dictionary

Using `items()` 

```python

# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin',
          'norway':'oslo', 'italy':'rome', 'poland':'warsaw', 'austria':'vienna' }
          
# Iterate over europe
for key, value in europe.items() :
     print("the capital of " + str(key) + " is " + str(value))

```


### Loop over Numpy array

```python

# Import numpy as np
import numpy as np


# For loop over np_height
for x in np_height:
    print(str(x) + " inches")

# For loop over np_baseball
for y in np.nditer(np_baseball):
    print(str(y))

```

### Loop over DataFrame (1)

Use `iterrows()` method

```python

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Iterate over rows of cars
for lab, row in cars.iterrows():
    print(lab)
    print(row)

```
### Loop over DataFrame (2)


```python

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Adapt for loop
for lab, row in cars.iterrows() :
    print(lab+": "+str(row['cars_per_cap']))

```

### Add column (1)


```python

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Code for loop that adds COUNTRY column
for lab, row in cars.iterrows():
    cars.loc[lab, "COUNTRY"] = row["country"].upper()


# Print cars
print(cars)

```

### Add column (2)


```python


# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Use .apply(str.upper)
cars["COUNTRY"] = cars["country"].apply(str.upper)

print(cars)

```



