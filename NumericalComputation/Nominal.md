把Categorical标签数据化  


# Integer Encoding

直接把类别转成序号，这种编码方式能天然表达category的顺序关系，适用于ordinal variable  
ordinal variable，是指有顺序关系的Categorical标签，例如first, second, third  

# One Hot Encoding

n个类别转成n维向量，第i个类别就把第i维置1  

```python
from sklearn.preprocessing import LabelEncoder
from sklearn.preprocessing import OneHotEncoder

label_encoder = LabelEncoder()
integer_encoded = label_encoder.fit_transform(values)
onehot_encoder = OntHotEncoder(sparse=False, categories='auto')
onehot_encoded = onehot_encoder.fit_transform(integer_encoded)
inverted = label_encoder.interse_transform(argmax(onehot.encoded[0,:]))
```