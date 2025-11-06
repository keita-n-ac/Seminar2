### 1
```python
N = int(input('Input Number -> '))
for i in range(N):
    print('Hello')
```

### 2
```python
N = int(input('Input Number -> '))
ans = 0
for i in range(N+1):
    ans += i

print(ans)
```

### 3
```python
N = int(input('Input Number -> '))
ans = 0
for i in range(1, N+1):
    if i % 2 == 0:
        ans += i

print(ans)
```

### 4
```python
N = int(input('Input Number -> '))
count = 0
for i in range(1, N+1):
    if i % 5 == 0:
        print(i)
        count += 1

print(count)
```

### 5
```python
while True:
    num = int(input("Enter a number: "))
    if num == 0:
        break
    print(num)
```

