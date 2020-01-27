# Bernoulli 分布
单个二值随机变量的分布

$$
P(X=1) = \phi \\
P(X=0) = 1 - \phi \\
P(X=a) = \phi^a(a-\phi)^{(1-a)} \\
E[x] = \phi \\
Var(x) = \phi(1-\phi)
$$

# Multinoulli 分布
具有k个不同状态的单个离散型随机变量的分布。  
分布由向量$$p \in [0,1]^{k-1}$$参数化  

$$
P(x = i) = p_i，i < k \\
P(x = k) = 1 - \sum_{i}p_i
$$
通常不计算方差和期望。  

# Logistic分布

定义：Logistic分布  
设X是连续随机变量，X服从逻辑分布是指X具有下列函数和密度函数：  
分布函数：  
$$
F(x) = P(X \le x) = \frac{1}{1+e^{-(x-\mu)/\gamma}}
$$
![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/6.png)  
密度函数：  
$$
f(x) = F^{'}(x) = \frac{e^{-(x-\mu)/\gamma}}{\gamma(1+e^{-(x-\mu)/\gamma})^2}
$$
![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/5.png)  
其中：$$mu$$为位置参数，$$\gamma$$是形状参数

# 正态分布（高斯分布）

$$
\mathcal N(x; \mu,\sigma^2) = \sqrt{-\frac {1}{2\pi\sigma^2}}exp(-\frac {1}{2\sigma^2}(x-\mu)^2)
$$

当对数据缺乏先验知识时，正态分布是默认的比较好的选择。  

**标准正态分布**：$$\mu=0, \sigma=1$$

![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/1.png)   

**多维正态分布**  

$$
\mathcal N(x; \mu,\Sigma^2) = \sqrt{-\frac {1}{(2\pi)^n|\Sigma|^2}}exp(-\frac {1}{2}(x-\mu)\Sigma (x-\mu)^T)
$$

公式中$$x, \mu$$都是向量，$$\Sigma$$是对称半正定矩阵

**各向同性(isotropic)高斯分布**：
$$
\Sigma = 标量 \times I
$$

# 指数分布

$$
p(x;\lambda)= 
\begin {cases}
 \lambda exp(-\lambda), & \text {if $x \geq$ 0} \\
 0, & \text{if $x \lt$ 0} 
\end{cases} 
$$

# Laplace分布

$$
Laplace(x;\mu, r) = \frac{1}{2r}exp(-\frac{|x-\mu|}{r})
$$

# Dirac分布

$$
p(x) = \delta(x-\mu) = 
\begin {cases}
\gt 0, & x = \mu \\
= 0, & x \neq \mu
\end {cases}    \\
\int p(x) = 1
$$

意义：只有在定义连续型随机变量的经验公布时，$$\delta(x)$$才有意义

**广义函数**：依据积分性质定义的数学对象  
