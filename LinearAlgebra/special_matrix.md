向量x与向量y**正交**：$$x^Ty=0$$  

向量x与向量y**标准正交**：$$x^Ty=0 且||x||_2=1且||y||_2=1$$    

**正交矩阵**:行向量和列向量分别标准正交的方阵，有以下性质：

$$
A^TA = AA^T = I \\
A^{-1} = A^T  \text 求逆计算代价小 \\
$$

**奇异矩阵**：有0特征值的矩阵。  
**正定矩阵**：所有特征值都是正数。
**半正定矩阵**：所有特征值非负，且：  
$$
\forall x, x^TAx \geq 0 \\
x^TAx - 0 \Rightarrow x=0
$$

**Hessian Matrix**：是一个多元函数的二阶偏导数构成的方阵，描述了函数的局部曲率。

**Jacobian矩阵**：在向量分析中，雅可比矩阵是函数的一阶偏导数以一定方式排列成的矩阵。  
假设$$F:R_m\rightarrow R_n$$是一个从n维欧氏空间映射到到m维欧氏空间的函数。这个函数由m个实函数组成：$$y_1(x_1,x_2,\cdots,x_m),y_2(x_1,x_2,\cdots,x_m),\cdots,y_n(x_1,x_2,\cdots,x_m)$$。这些函数的偏导数(如果存在)可以组成一个m行n列的矩阵，这个矩阵就是所谓的雅可比矩阵：
$$
\begin{bmatrix}
\frac{\partial y_1}{\partial x_1} & \cdots & \frac{\partial y_1}{\partial x_n} \\
\vdots & \ddots & \vdots \\
\frac{\partial y_m}{\partial x_1} & \cdots & \frac{\partial y_m}{\partial x_n} \\
\end{bmatrix}
$$
