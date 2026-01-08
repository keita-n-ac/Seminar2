### 問題1
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.arange(21)
y = 2 * x + 3
plt.plot(x, y)
plt.show()
```

### 問題2
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(0, 1, 11)
y = x * x
plt.xlim(0, 1)
plt.ylim(0, 1)
plt.plot(x, y)
plt.show()
```

### 問題3
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(0, 10, 11)
y = 5 * x
plt.plot(x, y, color='g', linewidth=4)
plt.show()
```

### 問題4
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(0.1, 20, 100)
y = 1 / x
plt.xlabel('x')
plt.ylabel('y')
plt.title('y = 1/x')
plt.plot(x, y)
plt.grid(True)
plt.show()
```

### 問題5
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(-5, 5, 100)
y1 = x
y2 = x * x
plt.plot(x, y1, linestyle='--', linewidth=4, label='y = x')
plt.plot(x, y2, linestyle=':', linewidth=4, label='y = x^2')
plt.legend()
plt.grid(True)
plt.show()
```

### 問題6
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(-np.pi, np.pi, 100)
y1 = np.sin(x)
y2 = np.cos(x)
plt.plot(x, y1, color='r', label='y = sin(x)', marker='o')
plt.plot(x, y2, color='b', label='y = cos(x)', marker='s')
plt.legend()
plt.show()
```

### 問題7
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(0, 5, 100)
y1 = 2 * x + 1
y2 = -x + 5
plt.plot(x, y1, color='r', label='y = 2x + 1')
plt.plot(x, y2, color='b', label='y = -x + 5')
plt.legend()
plt.show()
```

### 問題8
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.linspace(0, 10, 11)
y = x
plt.plot(x[::2], y[::2], color='r', linestyle='None', marker='D')
plt.show()
```

### 問題9
```python
import random
data = [0, 0, 0, 0, 0, 0]
for i in range(100):
    d = random.randint(1, 6)
    data[d - 1] += 1

print(data)
```

### 問題10
```python
import random
import matplotlib.pyplot as plt
data = []
for i in range(100):
    d = random.randint(1, 6)
    data.append(d)
plt.hist(data, bins=6)
plt.show()
```

### 問題11
```python
import numpy as np
data = np.random.randn(1000)
maxData = data[0]
minData = data[0]
for i in range(1, len(data)):
    if data[i] > maxData:
        maxData = data[i]
    if data[i] < minData:
        minData = data[i]

print(maxData, minData)
```

### 問題12
```python
import numpy as np
import matplotlib.pyplot as plt
x = np.linspace(0, 10, 100)
y1 = x
y2 = 10 - x
plt.plot(x, y1)
plt.plot(x, y2)
plt.show()
```

### 問題13
```python
import matplotlib.pyplot as plt
x = [1, 2, 3]
y = [120, 80, 150]
l = ['Item A', 'Item B', 'Item C']
plt.bar(x, y, tick_label=l)
plt.show()
```

### 問題14
```python
import matplotlib.pyplot as plt
x = [1, 2, 3]
y1 = [15, 20, 17]
y2 = [18, 12, 19]
l = ['Class A', 'Class B', 'Class C']
plt.bar(x, y1, tick_label=l)
plt.bar(x, y2, bottom=y1)
plt.show()
```

### 問題15
```python
import matplotlib.pyplot as plt
x = [1, 2, 3]
y1 = [15, 20, 17]
y2 = [18, 12, 19]
l = ['Class A', 'Class B', 'Class C']
plt.bar(x, y1, tick_label=l, color='b')
plt.bar(x, y2, bottom=y1, color='r')
plt.legend(['Male', 'Female'])
plt.show()
```

### 問題16
```python
import matplotlib.pyplot as plt
import numpy as np
data = np.random.randn(10000)
plt.hist(data, bins=50)
plt.show()
```

### 問題17
```python
import matplotlib.pyplot as plt
import numpy as np
data = np.random.randint(1, 7, 10000)
plt.hist(data, bins=6)
plt.show()
```

### 問題18
```python
import matplotlib.pyplot as plt
import numpy as np
data1 = np.random.randn(200)
data2 = np.random.randn(200)
plt.scatter(data1, data2, color='r', marker='D')
plt.show()
```

### 問題19
```python
import matplotlib.pyplot as plt
import numpy as np
x = np.random.randn(500)
y = np.random.randn(500)
data1x = []
data1y = []
data2x = []
data2y = []
for i in range(500):
    if x[i] > y[i]:
        data1x.append(x[i])
        data1y.append(y[i])
    else:
        data2x.append(x[i])
        data2y.append(y[i])
plt.scatter(data1x, data1y, color='r')
plt.scatter(data2x, data2y, color='b')
plt.show()
```

### 問題20
```python
import matplotlib.pyplot as plt
import numpy as np
data = np.linspace(-np.pi, np.pi, 201)
x = np.cos(data)
y = np.sin(data)
plt.scatter(x, y)
plt.axis('equal')
plt.grid(True)
plt.show()
```