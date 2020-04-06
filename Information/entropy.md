# 信息熵 entropy

**自信息**：表示一个事件的信息量，
$$
\begin{aligned}
I(x) = -\log P(x) && {1}
\end{aligned}
$$
如果公式（1）中的log以e为底，则I(x)单位是奈特（nats）。  
如果公式（1）中的log以2为底，则I(x)单位是比特（bit）或者香农（shannons）。  

**熵（香农熵，Shannon Entropy）**:表示整个概率分布的不确定性。  
$$
\begin{aligned}
H(x) = E_{x\sim P}[I(x)] && {2}
\end{aligned}
$$

根据[期望和方差](https://windmising.gitbook.io/mathematics-basic-for-ml/gai-shuai-lun/expectation_variance)中离散型变量期望的计算公式（公式1），可进一步得出：  
$$
\begin{aligned}
H(x) = -\sum_{i=1}^nP(x_i)\log P(x_i) && {3}
\end{aligned}
$$

公式(3)中：  
n: 该分布中x可以取n个不同的值  
$$P(x_i)$$为x取第i个值的概率
公式（2）和（3）都是基于公式（1）计算的，因此公式中的log也可以以e为底或者以2为底，以上下文环境为准。  

**条件熵**H(Y|X)：X给定条件下Y的条件概率分布的熵对X的数学期望  
$$
\begin{aligned}
H(Y|X) = \sum_{i=1}^nH(Y|X=x_i)P(X=x_i)
\end{aligned}
$$

**基尼指数**：  
$$
\begin{aligned}
Gini(p) = \sum^K p_k(1-p_k) = 1 - \sum^Kp_k^2
\end{aligned}
$$