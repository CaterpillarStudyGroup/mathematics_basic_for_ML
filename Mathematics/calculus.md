# 微分

![](/assets/images/8.png)  

$$
\begin{aligned}
dx = \Delta x  \\
dy = f'(x)dx   \\
\Delta y = dy + O(\Delta x)
f'(x) = \frac{dy}{dx}
\end{aligned}
$$

# 积分

![](/assets/images/9.png)  

$$
\int_a^bf(x)dx = \lim_{\lambda\rightarrow 0}\sum_{i=1}^nf(\epsilon_i)\Delta x
$$

说明：  
$\lambda\rightarrow 0$：划分越线越好  
$\sum_{i=1}^n$：所有子区间的面积之和  
$f(\epsilon_i)$：用子区间内一个点的y代表整个区间的y    
$\Delta x$：子区间的x  

# 微积分的基本定理

## 第一基本定理

设实函数f(x)在闭区间[a,b]上连续，如果   
$$
F(x) = \int_a^x f(t)dt
$$

那么F(x)可导，且$F'(x) = f(x)$

## 第二基本定理 牛顿-莱布尼茨公式

若函数f(x)在[a, b]上连续，且存在原函数$F'(x) = f(x)$，则f(x)在[a, b]上可积，且  
$$
\int_a^b f(x)dx = F(b) - F(a)
$$

## 积分中值定理

若函数f(x)在[a, b]上连续，则在[a, b]上至少存在一点$\xi$，使得：  
$$
\int_a^b f(x)dx = f(\xi)(b-a)
$$

