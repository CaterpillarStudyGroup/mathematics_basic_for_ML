# 指数加权平均

$$
V_t = \beta V_{t-1} + (1-\beta)\theta_t
$$

$\theta_t$代表真实测量数据  
$V_t \approx \frac{1}{1-\beta}$个过去的$\theta$的平均。  
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

公式中t代表当前时间，i代表距离t有多远  

$$
(1-\beta)^{\frac{1}{\beta}} = \beta^{(\frac{1}{1-\beta})} = \frac{1}{e} \approx 0.35
$$

当$i > \frac{1}{1-\beta}$时，$\theta_{t-i}$对Vt的影响很少（少于$\frac{1}{e}$），认为不重要，因此说$V_t \approx \frac{1}{1-\beta}$个过去的$\theta$的平均。

![](/assets/images/14.png)  
上面为原始数据，下面是权重。这张图让我想到了DSP里面的激励信号*原始信号，以前都无法理解信号里的卷积，现在看来好像是有点道理的。  

# 优点

目的是求过去n个值的平均值，相比于“过去n个值加以前再除以n”的方法，优点如下：  
1. low memory: 不需要真的存储过去的n个值。  
2. efficiency: 计算更简单，只是一个公式一行代码。  

# 修正偏差

目的：让指数加权平均的计算更准确  
![](/assets/images/13.png)  
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
2. Ng的视频