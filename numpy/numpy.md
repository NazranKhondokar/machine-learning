```python
import numpy as np
```

## NumPy Array with `Zeros()` Function


```python
np.zeros(5)
```




    array([0., 0., 0., 0., 0.])




```python
np.zeros((3,5), dtype = "int")
```




    array([[0, 0, 0, 0, 0],
           [0, 0, 0, 0, 0],
           [0, 0, 0, 0, 0]])



## NumPy Array with `Ones()` Function


```python
np.ones((3,4,5), dtype = "int")
```




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



## NumPy Array with `Full()` Function


```python
np.full((2,3), 6, dtype = "float")
```




    array([[6., 6., 6.],
           [6., 6., 6.]])



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




```python

```
