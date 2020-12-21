# 归一化 Normalized

把数据归一化[0,1]之间。  
需要知道数据的最大值和最小值。  
如果使用训练数据的最大值和最小值，则可能出现测试数据超出范围的情况。  
可以把超出范围的数据drop或者cutdown。  

sklearn实现：  

```python
from sklearn.preprocessing import MinMaxScaler

scaler = MinMaxScaler(feature_range=(0,1))
scaler = scaler.fit(values)
normalized = scaler.transform(values)
inversed = scaler.inverse_transform(normalized)
```

# 标准化 Standardize

把数据标准化为均值为0方差为1的数据。  
需要知道数据的均值和方差。  
通常使用训练数据的均值和方差。  

sklearn实现：  

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
scaler = scaler.fit(values)
normalized = scaler.transform(values)
inversed = scaler.inverse_transform(normalized)
```