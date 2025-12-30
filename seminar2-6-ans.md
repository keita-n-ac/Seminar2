### 01
```python
x = [10, 20, 30, 40, 50]
print(x[0])
print(x[2])
print(x[-1])
```

### 02
```python
x = [1, 2, 3, 4, 5]
x[0] = 100
x[1] += 200
print(x)
```

### 03
```python
a = []
for i in range(3):
    n = int(input('整数を入力してください'))
    a.append(n)
print(len(a))
```

### 04
```python
x = [10, 20, 30, 40]
x.insert(1, 15)
print(x)
x.remove(30)
print(x)
```

### 05
```python
x = [3, 6, 9, 12, 15]
for i in x:
    print(i)
```

### 06
```python
x = [5, 10, 15, 20, 25]

for i in range(len(x)):
    print('インデックス', i, ': 値', x[i])
```

### 07
```python
scores = [60, 70, 80, 90, 100]
print(sum(scores))
print(sum(scores)/len(scores))
```


### 08
```python
scores = [60, 70, 80, 90, 100]
count = 0
total = 0

for i in scores:
    total += i
    count += 1
print(total)
print(total/count)
```


### 09
```python
data = []

for i in range(5):
    n = int(input('整数を入力してください'))
    data.append(n)

print(min(data))
print(max(data))
```

### 10
```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(a[2:5])
print(a[:7])
print(a[4:])
```

### 11
```python
a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(a[0:10:2])
print(a[1:10:2])
```

### 12
```python
b = [10, 20, 30, 40, 50]
print(b[-1])
print(b[-2])
print(b[-3])
```

### 13
```python
x = []
for i in range(5):
    n = int(input('整数を入力してください'))
    x.append(n)
print(x)
print(x[::-1])
```

### 14
```python
N = int(input('正の整数を入力してください'))

nums = []
for i in range(1, N+1):
    nums.append(i)
print(nums)
print(sum(nums))
print(sum(nums)/len(nums))
```

### 15
```python
odds = []
for i in range(1, 101, 2):
    odds.append(i)

print(odds)
print(sum(odds))
print(sum(odds)/len(odds))
```

### 16
```python
scores = {'Tanaka': 80, 'Suzuki': 90, 'Sato': 75}
print(scores['Tanaka'])
print(scores['Suzuki'])
print(scores['Sato'])
```

### 17
```python
scores = {'Tanaka': 80, 'Suzuki': 90, 'Sato': 75}
scores['Yamada'] = 85
scores['Tanaka'] += 5
print(scores)
```

### 18
```python
prices = {'apple': 120, 'banana': 100, 'orange': 150}
del prices['banana']
print(prices)
```

### 19
```python
words = {'apple': 'りんご', 'dog': 'いぬ', 'cat': 'ねこ'}
s = input('英単語を入力してください')
if s in words:
    print(words[s])
else:
    print('その単語は登録されていません')
```

### 20
```python
N = int(input('学生の人数を入力してください'))
data = []

for i in range(N):
    s = int(input('点数を入力してください'))
    data.append(s)

print(data)
print(max(data))
print(min(data))
print(sum(data)/len(data))
```
