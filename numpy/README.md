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
---
## Array with `zeros` function
- In
```
np.zeros(5)
```
- Out
```python
array([0., 0., 0., 0., 0.])
```

- In
```
np.zeros((3,5), dtype = "int")
```
- Out
```python
array([[0, 0, 0, 0, 0],
       [0, 0, 0, 0, 0],
       [0, 0, 0, 0, 0]])
```
---
## Array with `ones` function
- In
```
np.ones((3,4,5), dtype = "int")
```
- Out
```python
array([[[1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1]],

       [[1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1]],

       [[1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1]]])
```
---
## Array with `full` function
- In
```
np.full((2,3), 6, dtype = "float")
```
- Out
```python
array([[6., 6., 6.],
       [6., 6., 6.]])
```
---
## Array with `arange` function
- In
```
np.arange(2, 10, dtype = "float")
```
- Out
```python
array([[6., 6., 6.],
       [6., 6., 6.]])
```
## NumPy Array with `Arange()` Function


```python
np.arange(2, 10, dtype = "float")
```




    array([2., 3., 4., 5., 6., 7., 8., 9.])



## NumPy Array with `Eye()` Function


```python
np.eye(3)
```




    array([[1., 0., 0.],
           [0., 1., 0.],
           [0., 0., 1.]])




```python
np.eye(3,2)
```




    array([[1., 0.],
           [0., 1.],
           [0., 0.]])




```python
np.eye(3,2,dtype="bool")
```




    array([[ True, False],
           [False,  True],
           [False, False]])



## NumPy Array with `Linspace()` Function


```python
np.linspace(10, 30, 10)
```




    array([10.        , 12.22222222, 14.44444444, 16.66666667, 18.88888889,
           21.11111111, 23.33333333, 25.55555556, 27.77777778, 30.        ])



## NumPy Array with `Random()` Function


```python
np.random.rand(5)
```




    array([0.04912221, 0.31058067, 0.24809702, 0.67342094, 0.81900648])




```python
np.random.rand(2, 3)
```




    array([[0.05620318, 0.71502624, 0.26362882],
           [0.79348239, 0.8062787 , 0.21943066]])




```python
np.random.randn(5)
```




    array([ 1.61992538, -0.47040122, -2.85078972, -0.13634668, -0.56320056])




```python
np.random.normal(20, 5, (4, 3))
```




    array([[26.97403092, 21.56144297, 18.8049518 ],
           [25.20092111, 26.4127337 , 28.2941984 ],
           [21.44260703, 27.65557638, 17.94579729],
           [17.20973714, 22.94490813, 15.66496286]])




```python
np.random.randint(0, 10, (4, 4))
```




    array([[7, 5, 8, 5],
           [5, 8, 1, 2],
           [9, 0, 2, 9],
           [3, 9, 7, 3]])



## NumPy Array `Reshape()` Function


```python
example = np.arange(1, 16)
```


```python
example
```




    array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14, 15])




```python
array = example.reshape(3, 5)
```


```python
array
```




    array([[ 1,  2,  3,  4,  5],
           [ 6,  7,  8,  9, 10],
           [11, 12, 13, 14, 15]])



// Getting the number of dimensions


```python
example.ndim
```




    1




```python
array.ndim
```




    2



## Identifying the Largest Element of a Numpy Array


```python
array = np.random.randint(0, 50, (4, 3))
```


```python
array
```




    array([[42, 10, 23],
           [ 7,  1, 36],
           [ 7, 36, 13],
           [13,  2, 29]])




```python
array.max()
```




    42



// max value index


```python
array.argmax()
```




    0



## Identifying the Largest Element of a Numpy Array


```python
array.min()
```




    1




```python
## min value index
```


```python
array.argmin()
```




    4



## Numpy Arrays `Concatenate()` Function


```python
array1 = np.array([1,2,3,4])
```


```python
array2 = np.array([5,6,7,8])
```


```python
np.concatenate([array1, array2])
```




    array([1, 2, 3, 4, 5, 6, 7, 8])




```python
array3 = np.arange(1,7).reshape(2,3)
```


```python
array3
```




    array([[1, 2, 3],
           [4, 5, 6]])




```python
array4 = np.array([[7,8,9],[10,11,12]])
```


```python
array4
```




    array([[ 7,  8,  9],
           [10, 11, 12]])




```python
np.concatenate([array3, array4])
```




    array([[ 1,  2,  3],
           [ 4,  5,  6],
           [ 7,  8,  9],
           [10, 11, 12]])




```python
np.concatenate([array3, array4], axis = 1)
```




    array([[ 1,  2,  3,  7,  8,  9],
           [ 4,  5,  6, 10, 11, 12]])



## Splitting One-Dimensional Numpy Arrays


```python
np.split(array, [3,5])
```




    [array([[42, 10, 23],
            [ 7,  1, 36],
            [ 7, 36, 13]]),
     array([[13,  2, 29]]),
     array([], shape=(0, 3), dtype=int64)]




```python
x, y, z = np.split(array, [3, 5])
```


```python
x
```




    array([[42, 10, 23],
           [ 7,  1, 36],
           [ 7, 36, 13]])




```python
y
```




    array([[13,  2, 29]])




```python
z
```




    array([], shape=(0, 3), dtype=int64)




```python
np.split(array, 4)
```




    [array([[42, 10, 23]]),
     array([[ 7,  1, 36]]),
     array([[ 7, 36, 13]]),
     array([[13,  2, 29]])]



## Splitting Two-Dimensional Numpy Arrays


```python
np.split(array, [1,3], axis = 1)
```




    [array([[42],
            [ 7],
            [ 7],
            [13]]),
     array([[10, 23],
            [ 1, 36],
            [36, 13],
            [ 2, 29]]),
     array([], shape=(4, 0), dtype=int64)]




```python
// horizontal split
```


```python
np.hsplit(array, 3)
```




    [array([[42],
            [ 7],
            [ 7],
            [13]]),
     array([[10],
            [ 1],
            [36],
            [ 2]]),
     array([[23],
            [36],
            [13],
            [29]])]




```python
np.hsplit(array, [1,3])
```




    [array([[42],
            [ 7],
            [ 7],
            [13]]),
     array([[10, 23],
            [ 1, 36],
            [36, 13],
            [ 2, 29]]),
     array([], shape=(4, 0), dtype=int64)]




```python
// vertical split
```


```python
np.vsplit(array, 4)
```




    [array([[42, 10, 23]]),
     array([[ 7,  1, 36]]),
     array([[ 7, 36, 13]]),
     array([[13,  2, 29]])]



## Splitting Two-Dimensional Numpy Arrays `Sort()` Function


```python
example = np.random.normal(30, 10, (4, 4))
```


```python
example
```




    array([[27.03802361, 35.22056023, 20.16865371, 22.85540356],
           [26.65872587, 18.71805371, 28.50734664, 12.37960792],
           [34.21900764, 37.53818275, 36.50627716, 30.77033107],
           [36.82730544,  9.45518368, 22.26713202, 44.4826718 ]])




```python
np.sort(example, axis = 1)
```




    array([[20.16865371, 22.85540356, 27.03802361, 35.22056023],
           [12.37960792, 18.71805371, 26.65872587, 28.50734664],
           [30.77033107, 34.21900764, 36.50627716, 37.53818275],
           [ 9.45518368, 22.26713202, 36.82730544, 44.4826718 ]])



## Indexing Numpy Arrays


```python
array[-1, -3]
```




    13




```python
array[2, 2]
```




    13



## Slicing Arrays


```python
array
```




    array([[42, 10, 23],
           [ 7,  1, 36],
           [ 7, 36, 13],
           [13,  2, 29]])




```python
array[3::2]
```




    array([[13,  2, 29]])




```python
array[:7:4]
```




    array([[42, 10, 23]])




```python
array[1:4,0:3]
```




    array([[ 7,  1, 36],
           [ 7, 36, 13],
           [13,  2, 29]])



#### Explanation
- Rows: The slicing starts at row index 1 and goes up to (but does not include) row index 4, so rows 1, 2, and 3 are selected.
- Columns: The slicing starts at column index 0 and goes up to (but does not include) column index 3, so columns 0, 1, and 2 are selected.


```python
array[0::2, 0::2]
```




    array([[42, 23],
           [ 7, 13]])



#### Explanation
- Rows: The slicing starts at row index 0 and selects every 2nd row, so it includes rows at indices 0 and 2.
- Columns: The slicing starts at column index 0 and selects every 2nd column, so it includes columns at indices 0 and 2.

## Solving Second-Degree Equations with NumPy
2X1 + X2 = 5
-3X1 + 6X2 = 0

```python
coefficient = np.array([[2,1],[-3,6]])
```


```python
coefficient
```




    array([[ 2,  1],
           [-3,  6]])




```python
output = np.array([5,0])
```


```python
output
```




    array([5, 0])




```python
np.linalg.solve(coefficient, output)
```




    array([2., 1.])
