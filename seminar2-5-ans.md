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
    for j in range(n - i + 1, 1, -1):
        print('*', end='')
    print('')
```

### 12
```python
for i in range(10):
    for j in range(10):
        print((i + j) % 10, end='')
    print('')
```

### 13
```python
n = int(input('奇数を入力してください'))
k = n // 2
for i in range(k+1):
    for j in range(k - i):
        print(' ', end='')
    for j in range(i * 2 + 1):
        print('*', end='')
    print('')
for i in range(k):
    for j in range(i+1):
        print(' ', end='')
    for j in range((k - i) * 2 - 1):
        print('*', end='')
    print('')
```

### 14
```python
n = int(input('自然数を入力してください'))
for i in range(n):
    for j in range(n - i):
        print(' ', end='')
    print('*', end='')
    if i == 0:
        print('')
    else:
        for j in range(2*i -1):
            if i == n - 1:
                print('*', end='')
            else:
                print(' ', end='')
        print('*')
```

### 15
```python
h = int(input('縦を入力してください'))
w = int(input('横を入力してください'))
for i in range(h):
    for j in range(w):
        if i == 0 or j == 0 or i == h-1 or j == w-1:
            print('#', end='')
        else:
            print(i-1, end='')
    print('')
```

### 16
```python
for i in range(10):
    for j in range(12):
        if j % 3 == 2:
            print('B', end=' ')
        else:
            print('A', end=' ')
    print('')
```

### 17
```python
n = int(input('サイズを入力してください'))

for i in range(n):
    for j in range(n):
        if i == j and i == n//2 and n % 2 == 1:
            print('×', end='')
        elif i == j:
            print('\\', end='')
        elif (i+j) == n-1:
            print('/', end='')
        else:
            print('.', end='')
    print('')
```

### 18
```python

```
