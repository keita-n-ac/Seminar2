### 問題1
```python
import math
print(math.pow(3, 4))
print(math.sqrt(144))
```

### 問題2
```python
import math as m
print(m.pow(10, 2))
```

### 問題3
```python
import random
print(random.randint(10, 20))
```

### 問題4
```python
import random
fruits = ['apple', 'banana', 'cherry', 'grape']
print(random.choice(fruits))
```

### 問題5
```python
import random
for i in range(5):
    print(random.randint(1, 100))
```

### 問題6
```python
import calendar
print(calendar.month(2025, 1))
```

### 問題7
```python
import numpy as np
a = [10, 20, 30, 40, 50]
a = np.array(a)
print(a)
print(type(a))
```

### 問題8
```python
import numpy as np
a = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
a = np.array(a)
print(a)
```

### 問題9
```python
import numpy as np
a = np.arange(10)
print(a)
```

### 問題10
```python
import numpy as np
a = np.arange(30, 0, -3)
print(a)
```

### 問題11
```python
import numpy as np
a = np.linspace(0, 100, 6)
print(a)
```

### 問題12
```python
import numpy as np
a = np.array([1, 2, 3, 4, 5])
print(a*10)
```

### 問題13
```python
import numpy as np
a = np.array([10, 20, 30])
b = np.array([1, 2, 3])
print(a - b)
```

### 問題14
```python
import numpy as np
a = np.array([4, 9, 16, 25])
print(np.sqrt(a))
```

### 問題15
```python
import numpy as np
a = np.array([-5, -2, 0, 3, 8])
print(np.abs(a))
```

### 問題16
```python
import numpy as np
data = np.arange(20)
print(data[5:10])
```

### 問題17
```python
import numpy as np
data = np.zeros(10)
data[3:7] = 99
print(data)
```

### 問題18
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.arange(0, 10, 0.1)
y = 2 * x
plt.plot(x, y)
plt.show()
```

### 問題19
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.arange(0, 10, 0.1)
y = 2 * x * x
plt.xlabel('Time')
plt.ylabel('Distance')
plt.plot(x, y)
plt.show()
```

### 問題20
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(-5, 5, 100)
y1 = x * x
y2 = x * x * x
plt.plot(x, y1)
plt.plot(x, y2)
plt.show()
```
