泰勒公式是将一个在$x=x_0$处具有n阶导数的函数f(x)利用关于$f(x-x_0)$的n次多项式来逼近函数的方法。  

# 一维的泰勒公式

若函数f(x)在包含$x_0$的某个闭区间[a,b]上具有n阶导数，且在开区间（a,b）上具有（n+1）阶导数，则对闭区间[a,b]上任意一点x，成立下式：  

$$
f(x) = \frac{f(x_0)}{0!} + \frac{f'(x_0)}{1!}(x-x_0) + \frac{f''(x_0)}{2!}(x-x_0)^2 + \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n + R_n(x)
$$

其中:  
x是一个标量。  
$f^{(n)}(x)$表示f(x)的n阶导数  
等号后的多项式称为函数f(x）在$x_0$处的泰勒展开式  
剩余的$R_n(x)$是泰勒公式的余项，是$(x-x_0)$n的高阶无穷小。  

# 高维的泰勒公式  


$$
f(x) = f(x_0) + (x-x_0)g + \frac{1}{2}(x-x_0)^\top H(x-x_0) + ...
$$

其中:  
$x$是一个向量  
g是f在$x_0$处的梯度向量，即$g_i = \frac{\partial f(x_0)}  {\partial x_i}$    
H是[Hessian矩阵](https://windmissing.github.io/mathematics_basic_for_ML/LinearAlgebra/special_matrix.html)，$H_{ij} = \frac{\partial^2}{\partial x_i \partial x_j}f(x_0) = \frac{\partial^2}{\partial x_j \partial x_i}f(x_0) = H_{ji}$，H是一个对称矩阵。  

# 泰勒公式二阶项的几何意义

当x非常接近$x_0$时，二阶以上的项可以忽略，只考虑前三项，分别是常数项、一阶项、二阶项。  
同时为了简化总是，认为x是一个标量。  
$$
f(x) = f(x_0) + (x-x_0)f'(x_0) + \frac{1}{2}(x-x_0)^2f''(x_0)
$$

![](/assets/images/2.png)  

根据公式的前两项画出来的是绿色的虚线（一个直线）。  
根据公式全部三项画出来的是蓝色的曲线（一个二次曲线）。  
蓝线与绿线的差异来自二阶项。  

# 泰勒公式二阶项的作用  

1. 牛顿法  
2. 分析[临界点](https://windmissing.github.io/mathematics_basic_for_ML/Mathematics/derivative.html)的类型  
