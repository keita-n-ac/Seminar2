### 問題1
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60}
s = pd.Series(scores)
print(s)
```

### 問題2
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60}
s = pd.Series(scores)
print(s.iloc[0])
print(s.iloc[-1])
print(s.iloc[0:2])
```

### 問題3
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60}
s = pd.Series(scores)
print(s['Jiro'])
print(s[['Taro', 'Saburo']])
```

### 問題4
```python
import pandas as pd
name = ['Taro', 'Jiro', 'Saburo']
score = [78, 98, 60]
data = pd.Series(score, index=name)
print(data)
```

### 問題5
```python
import pandas as pd
name = ['Taro', 'Jiro', 'Saburo']
score = [78, 98, 60]
data = pd.Series(score, index=name)
data['Shiro'] = 100
print(data)
```

### 問題6
```python
import pandas as pd
name = ['Taro', 'Jiro', 'Saburo']
score = [78, 98, 60]
data = pd.Series(score, index=name)
data['Shiro'] = 100
data = data.drop('Taro')
print(data)
```

### 問題7
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60, 'Shiro': 100, 'Goro': 59, 'Rokuro': 30}
s = pd.Series(scores)
print(s[s >= 60])
```

### 問題8
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60, 'Shiro': 100, 'Goro': 59, 'Rokuro': 30}
s = pd.Series(scores)
s = s[s >= 60]
s = s[s < 70]
print(s)
```

### 問題9
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60, 'Shiro': 100, 'Goro': 59, 'Rokuro': 30}
s = pd.Series(scores)
s = s[s >= 60]

print(s.sort_index())
print(s.sort_index(ascending=False))
print(s.sort_values())
print(s.sort_values(ascending=False))
```

### 問題10
```python
import pandas as pd
scores = {'Taro': 78, 'Jiro': 98, 'Saburo': 60, 'Shiro': 100, 'Goro': 59, 'Rokuro': 30}
s = pd.Series(scores)
s = s[s >= 60]

print(s.index)
print(s.values)
```

### 問題11
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}
data = pd.DataFrame(table)
print(data)
```

### 問題12
```python
import pandas as pd

row = {'Name': 'Taro', 'Score': 78, 'Grade': 'B'}

data = pd.DataFrame([row])
print(data)
```

### 問題13
```python
import pandas as pd
indexName = ['Name', 'Score', 'Grade']
data1 = ['Taro', 78, 'B']
data2 = ['Jiro', 98, 'AA']
data3 = ['Saburo', 60, 'C']
series1 = pd.Series(data1, index=indexName)
series2 = pd.Series(data2, index=indexName)
series3 = pd.Series(data3, index=indexName)
dataTable = pd.DataFrame([series1, series2, series3])
print(dataTable)
```

### 問題14
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}

data = pd.DataFrame(table)
newData = {'Name': 'Shiro', 'Score': 100, 'Grade': 'AA'}
# 1データなので[]を付ける
newTable = pd.DataFrame([newData])
dataTable = pd.concat([data, newTable], ignore_index=True)
print(dataTable)
```

### 問題15
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}

data = pd.DataFrame(table)
newData = {'Name': 'Shiro', 'Score': 100, 'Grade': 'AA'}
# 1データなので[]を付ける
newTable = pd.DataFrame([newData])
dataTable = pd.concat([data, newTable], ignore_index=True)
dataTable['Data'] = ['12/7', '12/7', '12/7', '12/7']
print(dataTable)
```

### 問題16
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}

data = pd.DataFrame(table)
newData = {'Name': 'Shiro', 'Score': 100, 'Grade': 'AA'}
# 1データなので[]を付ける
newTable = pd.DataFrame([newData])
dataTable = pd.concat([data, newTable], ignore_index=True)
dataTable['Data'] = ['12/7', '12/7', '12/7', '12/7']
print(dataTable.loc[[0, 1], ['Name']])
```

### 問題17
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo'],
  'Score': [78, 98, 60],
  'Grade': ['B', 'AA', 'C']
}

data = pd.DataFrame(table)
newData = {'Name': 'Shiro', 'Score': 100, 'Grade': 'AA'}
# 1データなので[]を付ける
newTable = pd.DataFrame([newData])
dataTable = pd.concat([data, newTable], ignore_index=True)
dataTable['Data'] = ['12/7', '12/7', '12/7', '12/7']
print(dataTable.iloc[[1, 2], [1, 2]])
```

### 問題18
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo', 'Shiro', 'Goro'],
  'Score': [78, 98, 60, 100, 59],
  'Grade': ['B', 'AA', 'C', 'AA', 'D']
}

data = pd.DataFrame(table)

print(data.at[4, 'Name'])
data.at[4, 'Name'] = 'Rokuro'
data.at[4, 'Score'] += 30
data.at[4, 'Grade'] = 'A'
print(data)
```

### 問題19
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo', 'Shiro', 'Goro'],
  'Score': [78, 98, 60, 100, 59],
  'Grade': ['B', 'AA', 'C', 'AA', 'D']
}

data = pd.DataFrame(table)

data.at[4, 'Name'] = 'Rokuro'
data.at[4, 'Score'] += 30
data.at[4, 'Grade'] = 'A'

difData1 = data.drop(1)
print(difData1)

difData2 = data.drop([1, 2])
print(difData2)

difData3 = data.drop('Score', axis=1)
print(difData3)

difData4 = data.drop(['Score', 'Grade'], axis=1)
print(difData4)
```

### 問題20
```python
import pandas as pd

table = {
  'Name': ['Taro', 'Jiro', 'Saburo', 'Shiro', 'Goro'],
  'Score': [78, 98, 60, 100, 59],
  'Grade': ['B', 'AA', 'C', 'AA', 'D']
}

data = pd.DataFrame(table)

data1 = data.sort_values(by='Score', ascending=False)
print(data1)

data2 = data.loc[data['Grade'] == 'AA']
print(data2)

data3 = data.loc[data['Score'] >= 60]
print(data3)

data4 = data.sort_values(by=['Grade', 'Name'], ascending=True)
print(data4)
```