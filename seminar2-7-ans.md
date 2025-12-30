### 問題1
```python
scores = (70, 85, 90, 60, 75)
print('要素数: ' + str(len(scores)))
print('合計値: ' + str(sum(scores)))
print('平均値: ' + str(sum(scores)/len(scores)))
```

### 問題2
```python
data = [1, 2, 2, 3, 3, 3]
data = tuple(data)
print(data)
```

### 問題3
```python
fruits = ['apple', 'banana', 'apple', 'orange', 'banana']
fruits = set(fruits)
print(fruits)
```

### 問題4
```python
numbers = {10, 20, 30}
print('変更前: ', numbers)
numbers.add(40)
print('追加後: ', numbers)
numbers.remove(10)
print('削除後: ', numbers)
```

### 問題5
```python
a = {1, 2, 3, 4, 5}
b = {3, 4, 5, 6, 7}

print(a | b)
print(a & b)
print(a - b)
print(a ^ b)
```

### 問題6
```python
s = input('文字列を入力してください')
print(s[0])
print(s[-1])
print(len(s))
```

### 問題7
```python
name = 'sapporo'
print(name[:3])
print(name[4:])
print(name[::-1])
```

### 問題8
```python
s = input('単語を半角スペース区切りで入力してください')
print(s.split())
```

### 問題9
```python
text = "red,blue,green,yellow"
ans = text.split(",")
print(ans)
print(len(ans))
```

### 問題10
```python
s = input('整数を半角スペース区切りで入力してください')
score = s.split()
total = 0
for i in score:
    total += int(i)

print(total)
```

### 問題11
```python
subjects = ['国語', '数学', '英語', '情報']
s = input('科目名を入力してください')

if s in subjects:
    print(s + 'はリストにあります')
else:
    print(s + 'はリストにありません')
```

### 問題12
```python
scores = ('C', 'B', 'AA', 'A')

if 'AA' in scores:
    print('AAを含んでいます．')
else:
    print('AAを含んでいません．')
```

### 問題13
```python
grades = {'A', 'B', 'C', 'D'}
s = input('アルファベットを入力してください')

if s in grades:
    print(s + 'を含んでいます')
else:
    print(s + 'を含んでいません')
```

### 問題14
```python
cityTelNum = {'札幌': '011', '千歳': '0123', '滝川': '0125', '岩見沢': '0126'}
city = input('都市名を入力してください')
if city in cityTelNum:
    print(city + 'の市外局番は' + cityTelNum[city] + 'です')
else:
    print('見つかりませんでした')
```

### 問題15
```python
a = [[1, 2, 3], [4, 5, 6]]

print(a)
print(a[0])
print(a[1][0])
print(a[1][2])
```

### 問題16
```python
table = []
for i in range(3):
    temp = []
    for j in range(3):
        temp.append(3*i+j+1)
    table.append(temp)

for i in table:
    print(i)
```

### 問題17
```python
table = []
for i in range(5):
    temp = []
    for j in range(5):
        temp.append(0)
    table.append(temp)

for i in table:
    print(i)
```

### 問題18
```python
table = []
for i in range(9):
    temp = []
    for j in range(9):
        temp.append((i+1) * (j+1))
    table.append(temp)

for i in table:
    print(i)

print(table[2][3])
```

### 問題19
```python
listA = [1, 2, 2, 3]
tupleB = (3, 3, 4)
setC = {4, 5}
print(set(listA))
print(list(tupleB))
print(tuple(setC))
```

### 問題20
```python
list1 = ['A', 'B', 'C']
list2 = ['D', 'E']
list3 = list1 + list2
print(list3)
```
