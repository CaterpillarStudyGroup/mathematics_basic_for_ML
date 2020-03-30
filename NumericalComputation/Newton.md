牛顿法基于[泰勒公式](https://windmissing.github.io/mathematics_basic_for_ML/Mathematics/Formula/taylor.html)和[Hessian矩阵](https://windmissing.github.io/mathematics_basic_for_ML/LinearAlgebra/special_matrix.html)的应用。  

# 牛顿法的推导  

将损失函数$f(x)$在$x_0$处用泰勒公式展开，并保留到二阶项，得：  
$$
f(x) = f(x_0) + (x-x_0)g + \frac{1}{2}(x-x_0)^\top H(x-x_0) + ...
$$

牛顿法的思想是“直接找到令g=0”的位置。  
方法是对f(x)在$x_0$处的偏导并令所有偏导为0。  

$$
\begin{aligned}
f'(x) & = & \nabla_x f(x_0) & + & \nabla_x (x-x_0)g & + & \nabla_x \frac{1}{2}(x-x_0)^\top H(x-x_0)    \\
& = & 0 & + & g & + & H(x-x_0) 
\end{aligned}
$$

令f'(x)=0得：  
$$
x = -H^{-1}g + x_0
$$

# 牛顿法 VS 梯度下降法  

牛顿法：$x = -H^{-1}g + x_0$  
梯度下降法：$x =  -\eta g + x_0$

牛顿法相对于梯度下降法的改进，是将学习率变成了Hessian矩阵的逆。  
$H^{-1}$的作用：  
1. 改变梯度的方向  
2. 决定了step的size

# 举个例子

![](/assets/images/3.png)

假设loss function为图中的黑线。  
取x0的位置，按泰勒公式展开，保留前三项，得到红色曲线。  
红色曲线是二次曲线，可直接计算出来它的最小值处为x1。  
令x1为新的x0，开始下一轮迭代。  
如果f(x)本身就是二次曲线，牛顿法可以一步到位。  

# 牛顿法的缺点

1. $H^-1$的计算量大  
2. 这种方法只能保证找到f'(x)=0的点。但这种点不一定是minima。也有可能是maxima或者saddle point。  
![](/assets/images/4.png)  

因此，牛顿法不适用于深度学习。  