# Pandas 理解度チェック用 プログラム作成練習問題（全20題）

本資料は、Pandas（Series / DataFrame）の基本操作を理解しているかを確認するための  
プログラム作成練習問題である。  
写経ではなく、自分でコードを書くこと。
内容は以下のURL（ https://github.com/keita-n-ac/ml-ex/blob/main/lec11.ipynb ）となります．
---

## Level 1：Series の作成・参照

### 問題1
次の辞書から Series `s` を作成し、表示せよ。  

`scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60}`

---

### 問題2
問題1の Series `s` について、次を出力せよ。

- `s.iloc[0]` の値  
- `s.iloc[-1]` の値  
- `s.iloc[0:2]` の中身（Series）

---

### 問題3
問題1の Series `s` について、次を出力せよ。

- キー `'Jiro'` の値  
- キー `'Taro'` と `'Saburo'` をまとめて取り出した Series

---

### 問題4
次の2つのリストから Series を作成し、表示せよ。

- `name = ['Taro', 'Jiro', 'Saburo']`  
- `score = [78, 98, 60]`

※ `score` を値、`name` を index にすること。

---

## Level 2：Series の追加・削除・フィルタリング・ソート

### 問題5
問題1の Series `s` に、次を追加して表示せよ。

- `'Shiro' : 100`

---

### 問題6
問題5で作った Series から、キー `'Taro'` を削除した Series を作成し、表示せよ。

---

### 問題7
次の Series を作成し、60以上のデータだけを取り出して表示せよ。

`scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60, 'Shiro': 100, 'Goro': 59, 'Rokuro': 30}`

---

### 問題8
問題7の Series から、60以上70未満のデータだけを取り出して表示せよ。  

※ `and` は使わず、条件を2段階で書くこと。

---

### 問題9
問題7の Series を次の条件でソートし、それぞれ表示せよ。

- インデックス昇順  
- インデックス降順  
- 値の昇順  
- 値の降順  

---

### 問題10
問題7の Series について、次を出力せよ。

- `s.index`  
- `s.values`  

---

## Level 3：DataFrame の作成

### 問題11
次の辞書から DataFrame `df` を作成し、表示せよ。

```python
table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}
```

---

### 問題12
次の辞書（1件データ）から DataFrame を作成し、表示せよ。

```python
row = {'Name': 'Taro', 'Score': 78, 'Grade': 'B'}
```

※ 1件の場合は `[]` を付けること。

---

### 問題13
次の条件で Series を3つ作成し、それらから DataFrame を作成せよ。

- index：`['Name', 'Score', 'Grade']`
- データ  
  - Taro, 78, B  
  - Jiro, 98, AA  
  - Saburo, 60, C  

---

## Level 4：DataFrame の追加・参照

### 問題14
問題11の DataFrame に、次の1行を追加せよ。

- `{'Name': 'Shiro', 'Score': 100, 'Grade': 'AA'}`  

※ `pd.concat(..., ignore_index=True)` を使うこと。

---

### 問題15
問題14の DataFrame に、新しい列 `Date` を追加せよ。

- 値：`['12/7', '12/7', '12/7', '12/7']`

---

### 問題16
問題15の DataFrame から、`loc` を使って次を取り出せ。

- インデックス `[0, 1]` の `Name` 列

---

### 問題17
問題15の DataFrame から、`iloc` を使って次を取り出せ。

- 行：1, 2  
- 列：Score, Grade  

---

### 問題18
次の DataFrame を作成し、`at` を使って操作せよ。

```python
table = {
  'Name': ['Taro', 'Jiro', 'Saburo', 'Shiro', 'Goro'],
  'Score': [78, 98, 60, 100, 59],
  'Grade': ['B', 'AA', 'C', 'AA', 'D']
}
```

操作内容：
1. インデックス4の `Name` を出力  
2. インデックス4の `Name` を `'Rokuro'` に変更  
3. インデックス4の `Score` に 30 を加算  
4. インデックス4の `Grade` を `'A'` に変更  
5. DataFrame 全体を表示  

---

## Level 5：削除・ソート・フィルタリング

### 問題19
問題18の DataFrame を使い、次を作成せよ。

- インデックス1を削除  
- インデックス `[1,2]` を削除  
- `Score` 列を削除  
- `Score` と `Grade` 列を削除  

---

### 問題20（総合問題）
次の DataFrame を作成し、以下を行え。

```python
table = {
  'Name': ['Taro', 'Jiro', 'Saburo', 'Shiro', 'Goro'],
  'Score': [78, 98, 60, 100, 59],
  'Grade': ['B', 'AA', 'C', 'AA', 'D']
}
```

1. `Score` を降順でソート  
2. `Grade == 'AA'` の行を抽出  
3. `Score >= 60` の行を抽出  
4. `Grade` → `Name` の優先順位で昇順ソート  

---

## 注意
- `import pandas as pd` を使用すること  
- Series と DataFrame の違いを意識すること  
- `loc / iloc / at` の使い分けを意識すること  
