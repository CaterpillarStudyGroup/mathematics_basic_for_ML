# 函数

**实变函数**:以实数作为自变量的函数叫做实变函数。 

**仿射函数**，即最高次数为1的多项式函数。常数项为零的仿射函数称为线性函数。

**凸函数**:  
![](https://bkimg.cdn.bcebos.com/pic/0dd7912397dda14415d2ffbebcb7d0a20df486e7?x-bce-process=image/watermark,g_7,image_d2F0ZXIvYmFpa2UxNTA=,xp_5,yp_5)  
凸函数的形状像一个碗。  
设f为定义在区间I上的函数，若对I上的任意两点x1、x2，和任意的实数$\lambda$，总有  
$$
f(\lambda x_1 + (1-\lambda)x_2) \le \lambda f(x_1) + (1-\lambda)f(x_2)
$$

通俗点说，就是在函数上任意取两个点，这两个点连成的一条直线。在这两点之间的区间内，这条直线永远在函数的上方。  

**泰勒公式**：泰勒公式是将一个在$$x=x_0$$处具有n阶导数的函数f(x)利用关于$$f(x-x_0)$$的n次多项式来逼近函数的方法。
若函数f(x)在包含$$x_0$$的某个闭区间[a,b]上具有n阶导数，且在开区间（a,b）上具有（n+1）阶导数，则对闭区间[a,b]上任意一点x，成立下式：  
- 一维的泰勒公式：x是一个标量  

$$
f(x) = \frac{f(x_0)}{0!} + \frac{f'(x_0)}{1!}(x-x_0) + \frac{f''(x_0)}{2!}(x-x_0)^2 + \frac{f^{(n)}(x_0)}{n!}(x-x_0)^n + R_n(x)
$$

其中，$$f^{(n)}(x)$$表示f(x)的n阶导数，等号后的多项式称为函数f(x）在$$x_0$$处的泰勒展开式，剩余的$$R_n(x)$$是泰勒公式的余项，是$$(x-x_0)$$n的高阶无穷小。  
- 高维的泰勒公式：$\theta$是一个向量   
$$
f(\theta) = f(\theta^0) + (\theta-\theta^0)g + \frac{1}{2}(\theta-\theta^0)^\top H(\theta-\theta^0) + ...
$$

其中，g是f在$\theta^0$处的梯度向量，即$g_i = \frac{\partial f(\theta^0)}  {\partial \theta_i}$    
H是Hessian矩阵，$H_{ij} = \frac{\partial^2}{\partial \theta_i \partial \theta_j}f(\theta^0) = \frac{\partial^2}{\partial \theta_j \partial \theta_i}f(\theta^0) = H_{ji}$，H是一个对称矩阵。  

**闭式解（closed form solution）**：也叫解析解(analytical solution)，就是一些严格的公式,给出任意的自变量就可以求出其因变量,也就是问题的解, 他人可以利用这些公式计算各自的问题。**

**凸优化（convex optimization）**，或叫做凸最优化，凸最小化，是数学最优化的一个子领域，研究定义于凸集中的凸函数最小化的问题。