# 似然

假设真实存在一组数据集X = {x1, x2 , ..., xm}  
X服从概率分布$$p(x|\theta)$$，参数$$\theta$$未知。  
那么似然为真实存在的数据X发生的概率。用带参数$$\theta$$的函数来表示这个概率为：  
$$
P(X;\theta) = P(x^{(1)}|\theta)P(x^{(2)}|\theta)\cdots P(x^{(m)}|\theta) \tag {1}
$$

# 最大似然估计

由公式（1）知X发生的可能性与参数$$\theta$$有关。  
我们希望X发生的可能性最大。  
因此要找到一个合适的参数$$\theta$$，使得P(X;\theta)取到最大值。  
即  
$$
\theta = {\arg \max}_{\theta} P(X;\theta) \tag{2}
$$

公式（2）称为$$\theta$$的最大似然估计

# 对数似然估计

由于公式（1）是许多概率连乘的形式，使得公式（2）不便于计算。  
由于$$P(X;\theta)$$和$$\log P(X;\theta)$$具有相同的趋势，$${\arg \max}_{\theta} P(X;\theta)$$和$${\arg \max}_{\theta} \log P(X;\theta)$$是等价的。  
于是公式（2）转化为：  
$$
\begin{eqnarray}
\theta & = & {\arg \max}_{\theta} \log P(X;\theta) \\
& = & {\arg \max}_{\theta} \sum_{i=1}^m \log P(X^{(i)};\theta) \tag{3}
\end{eqnarray}
$$

公式（2）称为最大对数似然估计  

# 期望

同理，$${\arg \max}_{\theta} \log P(X;\theta)$$和$${\arg \max}_{\theta} \frac{1}{m}\log P(X;\theta)$$是等价的

于是公式（3）又转化成：  
$$
\begin{eqnarray}
\theta & = & {\arg \max}_{\theta} \sum_{i=1}^m \log P(X^{(i)};\theta) \\
& = & {\arg \max}_{\theta} \frac{1}{m}\log P(X;\theta) \\
& = & {\arg \max}_{\theta} \sum_{i=1}^m \hat p(x^{(i)};\theta) \log p(x^{(i)};\theta) \tag {4}  \\
& = & {\arg \max}_{\theta} E_{X \sim \hat p_{data}} \log p_{model}(x;\theta) \tag {5}
\end{eqnarray}  
$$

说明：  
公式（4）（5）中的$$\hat p$$或$$\hat p_{data}$$代表样本的真实概率  
公式（4）（5）中的$$p$$或$$\hat p_{model}$$代表模型预测的概率  

# 交叉熵

公式（4）可以看是经验分布$$\hat p$$和模型分布$$p$$之间的差异，这种形式称为交叉熵。  

# KL离散度

两个分布差异程度可以用DL离散度表示。  
$$
D_{KL} = E[\log p1 - \log p2]
$$
p1为经验分布，与模型与无关。  
因此最小化KL离散度就是要最小化$$-E[\log p2]$$，即$$-E[\log p_{model}(x)]$$