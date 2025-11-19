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

### 14
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

### 15
```python
N = int(input('Input positive integer: '))
count = 0
for i in range(1, N+1):
    if i % 3 == 0 and i % 7 == 0:
        count += 1
        print(i)
print('count =', count)
```

### 16
```python
N = int(input('Input positive integer: '))
for i in range(1, 10):
    print(i, '×', N, '=', i * N)
```

### 17
```python
N = int(input('Input positive integer: '))
isPrime = True
for i in range(2, N):
    if N % i == 0:
        isPrime = False
        break

if isPrime == True:
    print('Prime')
else:
    print('Composite')
```

### 18
```python
N = int(input('Input positive integer: '))
count = 0
for i in range(1, N):
    if i == 1:
        continue
    elif i == 2:
        count += 1
        continue
    isPrime = True
    for j in range(2, i):
        if i % j == 0:
            isPrime = False
            break
    if isPrime == True:
        count += 1

print(count)
```

### 19
```python
a = int(input('Input positive integer: '))
b = int(input('Input positive integer: '))

ans = 1
i = 2
while i <= a:
    if a % i == 0 and b % i == 0:
        ans = i
    i += 1

print(ans)
```

### 20
```python
s = input('Input string: ')
N = int(input('Input positive integer: '))

ans = ''
for i in range(N):
    ans += s
print(ans)
```

### 21
```python
N = int(input('Input positive integer: '))
ans = ''
for i in range(N):
    print('*' * (i+1))
```

### 22
```python
N = int(input('Input positive integer: '))
ans = ''
for i in range(N):
    print(' ' * (N - i - 1) + '*' * (i + 1))
```

### 23
```python
N = int(input('Input positive integer: '))
for i in range(N):
    for j in range(i + 1):
        print(j + 1, end='')
    print()
```

### 24
```python
N = int(input('Input positive integer: '))
for i in range(1, N+1):
    if i % 15 == 0:
        print('FizzBuzz')
    elif i % 3 == 0:
        print('Fizz')
    elif i % 5 == 0:
        print('Buzz')
    else:
        print(i)
```

### 25
```python
max_len = 0
current_len = 0
prev = 0

while True:
    n = int(input())  # 整数を1つ読み込む
    if n == 0:
        # 0 が来たら入力終了
        break
    if prev == 0:
        # 最初の1個目
        current_len = 1
    else:
        if n > prev:
            # 前の値より大きい → 増加が続いている
            current_len += 1
        else:
            # 増加が途切れた → 新しい区間を開始
            current_len = 1
    # 最大長を更新
    if current_len > max_len:
        max_len = current_len
    prev = n  # 今読んだ値を「前の値」として覚えておく

print('max_len =', max_len)
```
