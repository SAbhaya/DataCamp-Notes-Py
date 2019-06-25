# Intermediate Python for Data Science

## Chapter 2 - Dictionaries & Pandas

### Motivation for dictionaries


```python

# Definition of countries and capital
countries = ['spain', 'france', 'germany', 'norway']
capitals = ['madrid', 'paris', 'berlin', 'oslo']

# Get index of 'germany': ind_ger
ind_ger = countries.index('germany')

# Use ind_ger to print out capital of Germany
print(capitals[ind_ger])

```

### Create dictionary

Template

```python
my_dict = {
   "key1":"value1",
   "key2":"value2",
}
```
Use srings only above.

```python

# Definition of countries and capital
countries = ['spain', 'france', 'germany', 'norway']
capitals = ['madrid', 'paris', 'berlin', 'oslo']

# From string in countries and capitals, create dictionary europe
europe = { 'spain':'madrid', 'france':'paris', 'germany':'berlin', 'norway':'oslo' }

# Print europe
print(europe)

```

### Access dictionary

```python

# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin', 'norway':'oslo' }

# Print out the keys in europe
print(europe.keys())

# Print out value that belongs to key 'norway'
print(europe['norway'])

```

output:
    dict_keys(['germany', 'spain', 'norway', 'france'])
    oslo





