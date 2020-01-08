# 数据预处理

## 归一化 normalization
把所有数据映射到0-1之间

$$
x_{scale} = \frac {x - x_{min}}{x_{max} - x_{min}}
$$

适用于分布有明显边界的情况，受outlier影响较大  

## 标准化 standardization

把所有数据归一到均值为0方差为1的分布中  
数据分布没有明显的边界，有可能存在极端的数据值

$$
x_{scale} = \frac {x-x_{mean}}{S}
$$
其中S是标准差