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

### 9
```python
num = int(input('Input positive integer: '))
after = 0
before = num
if num > 0:
    while num > 0:
        after = (after * 10) + (num % 10)
        num //= 10
else:
    print('Error')

if before == after:
    print('Yes')
else:
    print('No')
```

### 10
```python
num = int(input('Input positive integer: '))
count = 0

for i in range(1, num + 1):
    if num % i == 0:
        count = count + 1
        print(i)

print('count =', count)
```

### 11
```python
num = int(input('Input positive integer: '))
ans = 0
for i in range(1, num + 1):
    ans += i ** 3

print(ans)
```

### 12
```python
num = int(input('Input positive integer: '))
for i in range(1, num + 1):
    if i % 2 == 0:
        continue
    print(i)
```

### 13
```python
num = int(input('Input positive integer: '))
for i in range(1, num + 1):
    if i % 2 == 0:
        continue
    print(i)
```

### 14
```python
max = 0
min = 0
sum = 0

for i in range(5):
    num = int(input('Input integer: '))
    if i == 0:
        max = num
        min = num
    else:
        if num > max:
            max = num
        if num < min:
            min = num
    sum += num

print('min =', min)
print('max =', max)
print('sum =', sum)
```

### 15
```python
K = int(input('Input integer: '))

if K == 1:
    print('0')
elif K == 2:
    print('0 1')
elif K >= 3:
    print('0 1 ', end='')
    a1 = 0
    a2 = 1
    for i in range(K - 2):
        a2, a1 = a1 + a2, a2
        print(a2, end=' ')
else:
    print('Error')
```
