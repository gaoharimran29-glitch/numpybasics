# NumPy Practice Solutions (Q1–Q10)

This repository contains beginner-level **NumPy interview & practice questions** with their solutions.  
Below are the first 10 solved questions with explanations and code.

---

## 1. Create a 1D NumPy array of first 20 natural numbers
```python
import numpy as np
x = np.arange(1, 21, 1)
print(x)
```

## 2. Create a NumPy array of shape (3,3) with all True values
```python
import numpy as np
x = np.ones((3,3), dtype=bool)
print(x)
```

## 3. Generate an array of 10 random integers between 1 and 100
```python
import numpy as np
x = np.random.randint(1, 100, 10)
print(x)
```

## 4. Create a 1D array of 50 evenly spaced numbers between 0 and 5
```python
import numpy as np
x = np.linspace(0, 5, 50)
print(x)
```

## 5. Check the shape and datatype of a NumPy array
```python
import numpy as np
x = np.array([10, 20, 40, 50])
print(x.shape)   # returns (4,)
print(x.dtype)   # returns dtype('int64') or int32 based on system
```

## 6. Create a 2D array of zeros of shape (4,5)
```python
import numpy as np
x = np.zeros((4,5))
print(x)
```

## 7. Create a 3x3 identity matrix
```python
import numpy as np
x = np.eye(3, 3)
print(x)
```

## 8. Generate an array of 100 random floats from a normal distribution
```python
import numpy as np
x = np.random.randn(100)
print(x)
```

## 9. Convert a Python list [1,2,3,4] into a NumPy array
```python
import numpy as np
x = [1,2,3,4]
y = np.array(x)
print(y)
```

## 10. Difference between np.array() and np.asarray()
```python
import numpy as np

# np.array() - makes a copy by default
lst = [1, 2, 3]
x = np.array(lst)
lst[0] = 99
print(x)   # output: [1 2 3], change NOT reflected

# np.asarray() - makes a view if input is already ndarray
arr = np.array([1, 2, 3])
x = np.asarray(arr)
arr[0] = 99
print(x)   # output: [99 2 3], change reflected

# If list is passed, np.asarray() also makes a copy (like np.array)
lst = [1, 2, 3]
x = np.asarray(lst)
lst[0] = 99
print(x)   # output: [1 2 3], change NOT reflected
```

---
# NumPy Practice Solutions (Q11–Q20)

## 11. Extract the first 5 elements of a NumPy array
```python
import numpy as np
x = np.array([10,20,4,5,6,7,8,7])
print(x[:5])   # [10 20  4  5  6]
```

## 12. Reverse a NumPy array without slicing
```python
import numpy as np
x = np.array([10,20,4,5,6,7,8,7])
print(np.flip(x))   # reversed array
```

## 13. Extract all even numbers from a NumPy array
```python
import numpy as np
x = np.array([10,20,4,5,6,7,8,7])
print(x[x%2==0])   # [10 20  4  6  8]
```

## 14. Get the last row of a 2D array
```python
import numpy as np
x = np.array([[10,20,30],
              [5,6,7],
              [0,9,8]])
print(x[-1])   # [0 9 8]
```

## 15. Slice a 2D array to get a submatrix of shape (2,2)
```python
import numpy as np
x = np.array([[10,20,30],
              [5,6,7],
              [0,9,8]])
submatrix = x[:2, :2]
print(submatrix)
print(submatrix.shape)  # (2,2)
```

## 16. Replace all odd numbers in an array with -1
```python
import numpy as np
x = np.array([[10,20,30],
              [5,6,7],
              [0,9,8]])
x[x%2!=0] = -1
print(x)
```

## 17. Flatten a 2D array into 1D
```python
import numpy as np
x = np.array([[10,20,30],
              [5,6,7],
              [0,9,8]])
print(x.flatten())   # [10 20 30  5  6  7  0  9  8]
```

## 18. Extract every alternate element of an array
```python
import numpy as np
x = np.array([[10,20,30],
              [5,6,7],
              [0,9,8]])
print(x.flatten()[::2])   # alternate elements
```

## 19. Slice a 3D array along axis 1
```python
import numpy as np
x = np.array([[[10,20,30],
              [5,6,7],
              [0,9,8]]])
print(x[:, :2, :])   # taking first 2 rows along axis 1
```

## 20. Replace all values greater than 50 in an array with 50
```python
import numpy as np
x = np.array([[55,20,30],
              [53,6,7],
              [0,9,56]])
x[x>50] = 50
print(x)
```
