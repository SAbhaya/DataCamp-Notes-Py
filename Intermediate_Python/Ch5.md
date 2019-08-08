# Intermediate Python for Data Science

## Chapter 5 - Case Study: Hacker Statistics

### Random Number | Random flot

`seed()` - set the random seed -> results are reproducable between simulations.
`rand()` - if no argument -> gnerate a random float between 0 ~ 1

```python

# Import numpy as np
import numpy as np

# Set the seed
np.random.seed(123)

# Generate and print random float
print(np.random.rand())

```

### Roll the dice

`randint()` - function of `random` package. Generate a random integer.

Generate integer 4,5,6,7

```python

import numpy as np
np.random.randint(4,8)

```

```python

# Import numpy and set seed
import numpy as np
np.random.seed(123)

# Use randint() to simulate a dice
print(np.random.randint(1, 7))

# Use randint() again
print(np.random.randint(1, 7))

```

### Determine your next move

```python

# Numpy is imported, seed is set

# Starting step
step = 50

# Roll the dice
dice = np.random.randint(1,7)

# Finish the control construct
if dice <= 2 :
    step = step - 1
elif dice <=5 :
    step = step + 1
else :
    step = step + np.random.randint(1,7)

# Print out dice and step
print(dice)
print(step)

```


