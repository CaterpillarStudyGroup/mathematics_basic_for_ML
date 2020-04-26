**奇异矩阵**：有0特征值的矩阵。  

**（半）正定/负定矩阵**：是用来描述**对称矩阵**的。  
||正定矩阵|半正定矩阵|负定矩阵|半负定矩阵|
|---|---|---|---|---|
|对于任意非零向量x|$x\top Hx > 0$|$x\top Hx \ge 0$|$x\top Hx < 0$|$x\top Hx \le 0$|
|所有特征值|正|非负|负|非正|

**问：为什么所有特征值为正的对称矩阵一定是正定的？**  
答：令v是H的一个特征向量且v是单位向量，$\lambda$是v对应的特征值，可以算出：$v^\top H v = \lambda$  
令v1、v2是H的两个特征向量且v1、v2都是单位向量且v1、v2相互正交，并令x=a1v1+a2v2，可以算出$x^\top Hx = a_1^2\lambda_1 + a_2^2\lambda_2$   
继续拓展，任意向量x可以用H的所有特征向量的某种线性组合。  
假设$x=a_1v_1 + a_2v_2 + ... + a_n v_n$，则$x\top Hx = a_1^2\lambda_1 + a_2^2\lambda_2 + ... + a_n^2\lambda_n$

**Hessian Matrix**：是一个多元函数的二阶偏导数构成的方阵，描述了函数的局部曲率。
![](/assets/images/1.png)  
性质一：H矩阵是对称矩阵。  
性质二：  
当H是正定时，f在x处是极小值点。  
当H是负定时，f在x处是极大值点。  
当H是不定时，f在x处不是极值点。  
当H是半正定或半负定时，f在x处是可疑极值点。  

**Jacobian矩阵**：在向量分析中，雅可比矩阵是函数的一阶偏导数以一定方式排列成的矩阵。  
假设$$F:R_m\rightarrow R_n$$是一个从n维欧氏空间映射到到m维欧氏空间的函数。这个函数由m个实函数组成：$$y_1(x_1,x_2,\cdots,x_m),y_2(x_1,x_2,\cdots,x_m),\cdots,y_n(x_1,x_2,\cdots,x_m)$$。这些函数的偏导数(如果存在)可以组成一个m行n列的矩阵，这个矩阵就是所谓的雅可比矩阵：
$$
\begin{bmatrix}
\frac{\partial y_1}{\partial x_1} & \cdots & \frac{\partial y_1}{\partial x_n} \\
\vdots & \ddots & \vdots \\
\frac{\partial y_m}{\partial x_1} & \cdots & \frac{\partial y_m}{\partial x_n} \\
\end{bmatrix}
$$

另一种解释为：n维的向量x对m维的向量y的偏导为m*n的Jacobian矩阵。  