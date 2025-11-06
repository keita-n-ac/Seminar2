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

### 6
```python
ac = 0
count = 0

while True:
    num = int(input("Enter a number: "))
    count += 1
    ac += num
    if ac > 30:
        break

print('sum =', ac , ', count =', count)
```

### 7
```python
num = int(input('Input positive integer: '))
keta = 0
if num > 0:
    while num > 0:
        keta += 1
        num //= 10
else:
    print('Error')
print(keta, '桁')
```

### 8
```python
num = int(input('Input positive integer: '))
after = 0
if num > 0:
    while num > 0:
        after = (after * 10) + (num % 10)
        num //= 10
else:
    print('Error')
print(after)
```
