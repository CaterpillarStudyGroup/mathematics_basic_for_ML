# logistic sigmoid函数
$$
\sigma(x) = \frac{1}{1+\exp(-x)}
$$

![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/2.png)   

意义：
1. $$\sigma(x) \in (0, 1)$$  
2. 通常用来产生Bernoulli分布中的参数$$\phi$$  
3. 当|x|非常大时会饱和，饱和是指$$\sigma'(x)$$的变化非常缓慢。  

# softplus函数

$$
\zeta(x) = \log(1+\exp(x))
$$

![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/3.png)  

意义：  
1. $$\zeta(x) \in (0, +\infty)$$  
2. 用于产生高斯分布的$$\beta$$或$$\sigma$$参数，$$\beta = \frac{1}{\sigma^2}$$  
3. 是$$x_+ = max(0, x)$$函数是平滑形式  

有用性质：  

![](http://windmissing.github.io/images_for_gitbook/mathematics_basic_for_ML/4.png)  
