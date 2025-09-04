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

✅ These are the **first 10 solved questions** from the NumPy expert series.  
More questions will be added as I progress 🚀
