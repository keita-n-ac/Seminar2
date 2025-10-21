#### 1
```python
num = int(input('整数を入力してください'))
if num > 0:
    print('正の整数です')
else:
    print('正の整数ではありません')
```

#### 2
```python
num = int(input('整数を入力してください'))
if num % 2 == 0:
    print('偶数です')
else:
    print('奇数です')
```

#### 3
```python
num = int(input('整数を入力してください'))
if num % 3 == 0:
    print('3の倍数です')
```

#### 4
```python
num = int(input('整数を入力してください'))
if num % 5 == 0:
    print('5で割り切れます')
else:
    print('5で割り切れません')
```

#### 5
```python
num1 = int(input('1つ目の整数を入力してください'))
num2 = int(input('2つ目の整数を入力してください'))

if num1 > num2:
    print(num1, '>', num2)
elif num1 < num2:
    print(num1, '<', num2)
else:
    print(num1, '=', num2)
```

#### 6
```python
num = int(input('整数を入力してください'))
if num >= 10:
    print('大きい')
else:
    print('小さい')
```

#### 7
```python
score = int(input('点数を入力してください'))
if num >= 60:
    print('合格')
else:
    print('不合格')
```

#### 8
```python
num = int(input('整数を入力してください'))
if num == 0:
    print('ゼロ')
else:
    print('ゼロではありません')
```

#### 9
```python
cost = int(input('金額を入力してください'))
if cost >= 700:
    print('くじ引きできます')
```

#### 10
```python
num = int(input('整数を入力してください'))
if num % 7 == 0:
    print('7の倍数です')
```

#### 11
```python
num = int(input('整数を入力してください'))
if num >= 10 and num < 100:
    print('2桁の整数です')
```

#### 12
```python
age = int(input('年齢を入力してください'))
if age >= 20:
    print('成人です')
```

#### 13
```python
num = int(input('整数を入力してください'))
if num < 0:
    print('負の数です')
```

#### 14
```python
num = int(input('整数を入力してください'))
if num == 100:
    print('ジャスト100')
```

#### 15
```python
s = input('文字列を入力してください')
if s == 'Hello':
    print('挨拶成功')
```

#### 16
```python
num = int(input('整数を入力してください'))
if num > 0:
    print('正')
elif num == 0:
    print('0')
else:
    print('負')
```

#### 17
```python
a = int(input('整数1を入力してください'))
b = int(input('整数2を入力してください'))

if a > b:
    print('a > b')
elif a == b:
    print('a = b')
else:
    print('a < b')
```

#### 18
```python
score = int(input('スコアを入力してください'))

if score >= 90:
    print('A')
elif score >= 80:
    print('B')
elif score >= 70:
    print('C')
elif score >= 60:
    print('D')
elif score < 60:
    print('F')
```

#### 19
```python
num = int(input('整数を入力してください'))
if num % 2 == 0 and num % 3 == 0:
    print('6の倍数です')
```

#### 20
```python
d = int(input('距離を入力してください'))
if d >= 20 and d < 40:
    print('中距離')
```

#### 21
```python
age = int(input('年齢を入力してください'))

if age >= 0 and age <= 12:
    print('子供')
elif age >= 13 and age <= 19:
    print('ティーン')
elif age >= 20 and age <= 64:
    print('大人')
elif age >= 65:
    print('高齢者')
```

#### 22
```python
num = int(input('整数を入力してください'))
if num % 2 == 0 or num % 5 == 0:
    print('OK')
else:
    print('NG')
```

#### 23
```python
m = int(input('月を入力してください'))
if m == 2:
    print('28日または29日')
elif m == 1 or m == 3 or m == 5 or m == 7 or m == 8 or m == 10 or m == 12:
    print('31日')
elif m == 4 or m == 6 or m == 9 or m == 11:
    print('30日')
```

#### 24
```python
a = int(input('整数1を入力してください'))
b = int(input('整数2を入力してください'))
c = int(input('整数3を入力してください'))

if a == b and a == c:
    print('Equal')
```

#### 25
```python
num = int(input('整数1を入力してください'))
if num >= 10 and num <= 100:
    print('10以上100以下を満たす')
```
