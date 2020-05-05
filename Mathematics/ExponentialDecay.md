# 指数加权平均

$$
V_t = \beta V_{t-1} + (1-\beta)\theta_t
$$

$V_t$约等于$\frac{1}{1-\beta}$个过去的$\theta$的平均。  
当$\beta$较大时，V曲线抖动变小，但V曲线和$\theta$曲线相比往右偏移（适应更缓慢）。  
当$\beta$较小时，V曲线抖动变大，但V曲线与$\theta$曲线更贴近。  

# 指数衰减  

将Vt公式展开得：  
$$
\begin{aligned}
V_t &=& (1-\beta)\theta_t + (1-\beta)\beta\theta_{t-1} + (1-\beta)\beta^2\theta_{t-1} + \cdots \\
&=& \sum_{i=0}^t(1-\beta)\beta^i\theta_{t-i}
\end{aligned}
$$

每个$\theta$的系数为\beta的指数，因此称为指数加权平均。  
当有新的$\theta$过来时，旧的$\theta$呈指数衰减。  

# 优点

目的是求过去n个值的平均值，相比于“过去n个值加以前再除以n”的方法，优点如下：  
1. 不需要真的存储过去的n个值。  
2. 计算更简单，只是一个公式一行代码。  

# 修改偏差

目的：让指数加权平均的计算更准确  
![](/assets/images/Chapter8/7.png)  
图中绿线和紫线的$\beta$相同。其中绿线为做过修改的加权平均，紫线未做修正的加权平均。区别在于紫线的起点较低。  
修改方法为：
$$
V_t = \frac{V_t}{1-\beta^t}
$$  

当t比较小时，公式对Vt有很大的修改。  
当t比较大时，Vt几乎无修正效果。  

Note：修正只对初始阶段有效果。如果不care初始阶段的效果，可以不修正。  


# 参考资料  

1. https://blog.csdn.net/zhufenghao/article/details/80879260  
2. Ag的视频