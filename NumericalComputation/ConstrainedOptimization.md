**约束优化**是指在x的某些集合S中找到f(x)的最大值或最小值。  
集合S内的点称为s的可行点。  

求解方法：KKT  
KKT方法是将原始的约束优化问题转换为一无约束的优化问题。  

1. 将S描述为m个等式$$g^{(i)}(x)=0$$和n个不等式$$h^{(j)}(x)<0$$。  
2. 为每个约束引入新的变量$$\lambda_i$$和$$\alpha_j$$  
3. 定义广义Lagrangian函数为：  
$$
L(x,\lambda,\alpha) = f(x) + \sum_i \lambda_i g^{(i)}(x) + \sum_j \alpha_j h^{(j)}(x)
$$
4. 通过优化无约束的广义Lagrangian 解决约束最小化问题。以下两个公式具有相同的最优点集x。    
$$
\begin{aligned}
\min_x\max_{\lambda}\max_{\alpha,\alpha>0}L(x,\lambda,\alpha) && (1)\\
\min_{x\in S}f(x) && (2)
\end{aligned}
$$
在公式（1）中，保证可行点不是最佳，可行点范围内的最优点不变。  

[?]后面的不太懂