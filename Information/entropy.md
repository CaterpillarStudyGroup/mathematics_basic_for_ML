# 信息熵 entropy

自信息：表示一个事件的信息量，单位是奈特（nats）  
$$
I(x) = -\log P(x)
$$

熵（香农熵，Shannon Entropy）:表示整个概率分布的不确定性。  
$$
H(x) = E_{x\sim P}[I(x)]
$$

根据[期望和方差](https://windmising.gitbook.io/mathematics-basic-for-ml/gai-shuai-lun/expectation_variance)中离散型变量期望的计算公式（公式1），可进一步得出：  
$$
H(x) = -\sum_{i=1}^nP(x_i)\log P(x_i)
$$

公式中：  
n: 该分布中x可以取n个不同的值  
$$P(x_i)$$为x取第i个值的概率

