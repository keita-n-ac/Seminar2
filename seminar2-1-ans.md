### 解答例

##### Q1
- プログラム
```python
print(3 + 5 * 2)
```
- 出力
  - ``13``

##### Q2
- プログラム
```python
print((3 + 5) / 2)
```
- 出力
  - ``4.0``

##### Q3
- プログラム
```python
print(7 // 3)
print(7 % 3)
print(7 / 3)
```
- 出力
  - ``2``
  - ``1``
  - ``2.3333333333333335``

##### Q4
- プログラム
```python
print(type(4))
print(type(4.0))
print(type(4/2))
print(type(4//2))
```
- 出力
  - ``<class 'int'>``
  - ``<class 'float'>``
  - ``<class 'float'>``
  - ``<class 'int'>``
    - よって，``整数型，小数型，小数型，整数型``となる．

##### Q5
- プログラム
```python
print("py" + "thon" * 3)
```
- 出力
  - ``pythonthonthon``

##### Q6
- プログラム
```python
print('a' * 5 + 'b' * 2 + 'c')
```
- 出力
  - ``aaaaabbc``

##### Q7
- プログラム
```python
"123" + 456
```
- 出力
  - エラーが発生する．
    - 文字と整数の足し算なのでエラーになる

##### Q8
- プログラム
```python
x = int(input())
print(x + 100)
```
- 出力（``30``と入力した場合）
  - ``130``

##### Q9
- プログラム
```python
print(int(3.99))
print(float(10))
print(str(12.5))
```
- 出力
  - ``3``
  - ``10.0``
  - ``12.5``

##### Q10
- プログラム
```python
a = int(input())
print(a ** 3)
```
- 出力（``30``と入力した場合）
  - ``27000``

##### Q11
- プログラム
```python
tate = int(input())
yoko = int(input())
print('周の長さ: ', 2 * tate + 2 *yoko)
print('面積: ', tate * yoko)
```
- 出力（``2``, ``3``と入力した場合）
  - ``周の長さ:  10``
  - ``面積:  6``

##### Q12
- プログラム
```python
S = int(input())
h = S // 3600
m = (S % 3600) // 60
s = (S % 3600) % 60
print(h, ':', m, ':', s)
```
- 出力（``7281``と入力した場合）
  - ``2 : 1 : 21``

##### Q13
- プログラム
```python
a = 10

print('aの値は', a, 'です')          # 書き方1
print('aの値は ' + str(a) + ' です') # 書き方2
```
- 出力
  - ``aの値は 10 です``
  - ``aの値は 10 です``

##### Q14
- プログラム
```python
# 方法1
x = 7
y = -2

print('方法1')
print('交換前: x =', x, ', y =', y)
x, y = y, x
print('交換後: x =', x, ', y =', y)

# 方法2
x = 7
y = -2

print('方法2')
print('交換前: x =', x, ', y =', y)
temp = x
x = y
y = temp
print('交換後: x =', x, ', y =', y)
```
- 出力
  - ``方法1``
  - ``交換前: x = 7 , y = -2``
  - ``交換後: x = -2 , y = 7``
  - ``方法2``
  - ``交換前: x = 7 , y = -2``
  - ``交換後: x = -2 , y = 7``

##### Q15
- プログラム
```python
a += 5
b *= 3
c -= 10
d //= 2
e **= 4
```

##### Q16
- プログラム
```python
a = 2
a = a * 3 # a = 6
a += 4    # a = 10
a //= 3   # a = 3
print(a)
```
- 出力
  - ``3``

##### Q17
- プログラム
```python
print(type(8 / 2))
print(type(8 // 2))
print(type(3 + 4.0))
print(type("a" * 3))
```
- 出力
  - ``<class 'float'>``
  - ``<class 'int'>``
  - ``<class 'float'>``
  - ``<class 'str'>``
    - よって，``小数型, 整数型，小数型，文字列型``となる．

##### Q18
- プログラム
```python
print(1 + 2)
print(1　+　2)   # ← こちら
```
- 出力
  - 全角スペースを使っているためエラーになる

##### Q19
- プログラム
```python
total = 200 * 3 + 30 * 6
cost = int(total * 1.1)
print(cost)
```
- 出力
  - ``858``

##### Q20
- プログラム
```python
a = int(input('整数を代入してください'))
b = int(input('整数を代入してください'))

print(a + b) # 和
print(a - b) # 差
print(a * b) # 積
print(a / b) # 商
print(a % b) # 剰余
```
- 出力
  - ``7``
  - ``3``
  - ``10``
  - ``2.5``
  - ``1``
