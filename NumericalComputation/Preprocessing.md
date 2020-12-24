# 归一化 Normalize

把数据映射到[0,1]之间。  
适用于分布有明显边界的情况，需要知道数据的最大值和最小值，受outlier影响较大。      

$$
x_{scale} = \frac {x - x_{min}}{x_{max} - x_{min}}
$$

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

把数据映射到均值为0方差为1的分布中。  
数据分布没有明显的边界，有可能存在极端的数据值。但需要知道数据的均值和方差。  

$$
x_{scale} = \frac {x-x_{mean}}{S}
$$

通常使用训练数据的均值和方差。  

sklearn实现：  

```python
from sklearn.preprocessing import StandardScaler

scaler = StandardScaler()
scaler = scaler.fit(values)
normalized = scaler.transform(values)
inversed = scaler.inverse_transform(normalized)
```