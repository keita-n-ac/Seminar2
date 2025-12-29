### 01
```python
for i in range(4):
    for j in range(6):
        print('○', end='')
    print('')
```

### 02
```python
for i in range(4):
    for j in range(5):
        print(j, end='')
    print('')
```

### 03
```python
for i in range(5):
    for j in range(8):
        print(i, end='')
    print('')
```

### 04
```python
for i in range(10):
    for j in range(i+1):
        print(j, end='')
    print('')
```

### 05
```python
for i in range(10):
    for j in range(i+1):
        print(i, end='')
    print('')
```

### 06
```python
for i in range(10):
    for j in range(10-i+1, 1, -1):
        print('■', end='')
    print('')
```

### 07
```python
for i in range(10):
    for j in range(10-i, 1, -1):
        print(' ', end='')
    for j in range(i+1):
        print('*', end='')
    print('')
```

### 08
```python
for i in range(10):
    for j in range(10):
        if j % 2 == 0:
            print('■', end='')
        else:
            print('□', end='')
    print('')
```

### 09
```python
for i in range(10):
    for j in range(10):
        if (i + j) % 2 == 0:
            print('■', end='')
        else:
            print('□', end='')
    print('')
```

### 10
```python
for i in range(10):
    for j in range(10):
        if i == j:
            print(i, end='')
        else:
            print(' ', end='')
    print('')
```

### 11
```python
n = int(input('段数を入力してください'))

for i in range(n):
    for j in range(i+1):
        print('*', end='')
    print('')
```

### 12
```python

```
