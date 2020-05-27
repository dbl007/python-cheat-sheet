# Series

## Operators are performed by index

```python
import pandas as pd

data1 = pd.Series([5, 2, 3,7], index=['a', 'b', 'c', 'd'])
# a    5
# b    2
# c    3
# d    7

data2 = pd.Series([10, 11, 12, 13], index=['d', 'c', 'b', 'a'])
# d    10
# c    11
# b    12
# a    13

data1 + data2
# a    18
# b    14
# c    14
# d    17
```

## Sorting

Ascending

```python
data1 = pd.Series([5, 2, 3,7], index=['a', 'b', 'c', 'd'])
print(data1.sort_values())
```
```
b    2
c    3
a    5
d    7
```

Descending

```python
data1 = pd.Series([5, 2, 3,7], index=['a', 'b', 'c', 'd'])
print(data1.sort_values(ascending=False))
```

```
d    7
a    5
c    3
b    2
```