# Speciality of `numpy`

## Multiply matrix
- Input
```python
import numpy as np
x = np.array([1,3,5,7,9])
y = np.array([4,6,8,10,11])
x * y
```
- Output
```python
array([ 4, 18, 40, 70, 99])
```
---
## Type conversion
- Input
```python
new_variable = np.array([5.8, 9, 7, 5])
new_variable
```

- Output
```python
array([5.8, 9. , 7. , 5. ])
```

- Input
```python
new_variable2 = np.array([5.8, 9, 7, 5], dtype = "int")
```

- Output
```python
array([5, 9, 7, 5])
```
