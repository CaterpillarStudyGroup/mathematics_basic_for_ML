先通过Mulitinoulli分布选择一个组件分布（component distribution）。  
再从组件分布中选择一个样本。  
**潜变量**：不能直接观测到的变量，例如Mulitinoulli分布中的变量

# 一般混合模型

一般混合模型是指具有如下形式的概率分布模型：  
$$
P(y|\theta) = \sum_{k=1}^Ka_k\phi(y|\theta_k)
$$
其中：  
$$a_k$$是系数，$$a_k \ge 0$$，且$$\sum_{k=1}^Ka_k=1$$  
$$\phi(y|\theta_k)$$可以是概率分布密度。  

组件i的**先验概率**（prior probability）：$$a_i = P(c=i)$$  
组件i的**后验概率**（posterior probability），即观测到x之后组件i的概率：$$P(c=i|x)$$  

# 高斯混合模型 Gaussian misture model

当$$\phi(y|\theta_k)$$为高斯分布密度，即  
$$
\phi(y|\theta_k) = \frac{1}{\sqrt {2\pi}\sigma_k}\exp(-\frac{(y-\mu_k)^2}{2\sigma_k^2})  \\
\theta = (a1, a2, \cdots, a_k, \mu_1, \mu_2, \cdots, \mu_k, \sigma_1, \sigma_2, \cdots, \sigma_k)
$$
此时$$P(y|\theta)$$为高斯混合分布。  
每个组件分布都高斯分布，且有自己的$$\mu$$和$$\Sigma$$。  

高斯混合模型是概率密度的万能近似器（universal approximator），在这种意义下，任何平滑的概率密度都可以用具有足够多组件的高斯混合模型以任意精度来逼近。

特殊的高斯混合模型：  
限制每个组件的协方差矩阵为对角的或者各向同性的(标量乘以单位矩阵）。  
[?]各向同性

[TODO]cs229配置的数学部分有关于高斯混合模型的详细内容，还没做笔记。

# F函数

假设隐变量数据Z的概率分布为$$\hat P(Z)$$，定义分布$$\hat P$$与参数$$\theta$$的函数$$F(\hat P, \theta)$$如下：  
$$
F(\hat P, \theta) = E_{\hat P}[\log P(Y, Z|theta)] + H(\hat P)
$$
式中，$$H(\hat P) = -E_{\hat P}[\log \hat P(Z)]$$是分布$$\hat P(Z)$$的熵。  