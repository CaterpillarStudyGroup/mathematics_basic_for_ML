# 三角形式的傅利叶级数

周期为T、角频率为$\omega = \frac{2\pi}{T}$的周期信号x(t)，如果满足狄里赫利条件(Dirichlet condition)，则可以表达成为傅利叶级数。  

狄里赫利条件(Dirichlet condition):  
1. 任意一个周期内，有限个间断点  
2. 任意一个周期内，有限的极大值和极小值  
3. 任意一个周期内，绝对值可积  

傅利叶级数：  
$$
\begin{aligned}
x(t) &=& a_0 + \sum_{n=1}^\infty \{a_n\cos(n\omega t) + b_n\sin(n\omega t)\}   &&   (1)\\
a_0 &=& \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t)dt   \\
a_n &=& \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t)\cos(n\omega t)dt   &&  n \ge 1   \\
b_n &=& \frac{1}{T} \int_{-\frac{T}{2}}^{\frac{T}{2}} x(t)\sin(n\omega t)dt   &&  n \ge 1 
\end{aligned}
$$

其中$\int_{-\frac{T}{2}}^{\frac{T}{2}}$是指一个周期内的积分，也可以表示为$\int_{t_0}^{t_0+T}$  

[三角函数公式](https://windmissing.github.io/mathematics_basic_for_ML/Mathematics/Formula/trigonometric.html)

## 维度与频率

### 维度的理解

傅利叶级数中的每一个频率成分都是一个维度。  
傅利叶展开得到的是无穷维的内积空间。  
同一个频度的正弦项和余弦项是正交的。  
不同的频率的正弦项是正交的。  
不同的频率的余弦项是正交的。  

### 频率的理解

对于普通的周期信号，周期为T，关于这种信号的频率有两种理解：  
1. 频率是周期的倒数，因此频率为$\frac{1}{T}$  
2. 周期信号包含许多不同的频率的正弦信号，每个正弦成分的频率是$\frac{1}{T}$的整数倍。  

## 频率不变性

问：为什么用傅利叶级数表达周期信号？  
答：因为三角函数作为线性系统的输入时，具有频率不变性。  

例如某输入信号为$x(t) = \cos (\omega t)$，经过某线性系统后，会得到输出信号$y(t) = A \cos(\omega t - \theta)$  
对比输入信号和输出信号：  
频率不变 --- 频率不变性  
幅度改变 --- 幅频特性   
相位改变 --- 相频特性  
幅频特性和相频特性统称为频率特性。  

# 复指数形式的傅利叶级数

[欧拉公式](https://windmissing.github.io/mathematics_basic_for_ML/Mathematics/Formula/euler.html)代入公式（1）得：  
$$
x(t) = a_0 + \sum_{n=1}^\infty[\frac{a_n-jb_n}{2}\exp(jn\omega t) + \frac{a_n + jb_n}{2}\exp(-jn\omega t)]
$$

定义：  
$c_0 = a_0$：第一项  
$c_n = \frac{a_n-jb_n}{2}$：第二项中的第一项的系数  
$c_{-n} = \frac{a_n+jb_n}{2}$：第二项中的第二项的系数    
则：  
$$
\begin{aligned}
x(t) = \sum_{-\infty}^{\infty} C_n \exp(jn\omega t)  && (2)
\end{aligned}
$$

说明：  
1. 公式（2）称为复指数形式的傅利叶级数  
2. [?]x(t)是很不同频率的复指数函数叠加的结果？  
3. $C_n$和$C_{-n}$是共轭复数的关系  
4. 负频率只是一种数学结果，没有实际的物理意义  
